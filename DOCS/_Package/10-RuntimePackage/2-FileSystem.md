---
layout: default

parent: 10. Runtime Package
has_children: true

title: FileSystem Class
nav_order: 2
permalink: /package/runtimepackage/filesystem

---
{% assign img1 = "https://biz-collections.com/support/webpages/html/onlinemanual/browser/crs/core/core1.files/image001.gif" %}

# {{ page.title }}

---

This class operates the file system of the client PC.

**Default properties and ValueType**

The default property is [PathName](/package/runtimepackage/filesystem/properties/pathname). The ValueType specification is invalid.

**Virtual file name**

The FileSystem class treats file names as virtual file names. A virtual file name is a file name with limited access range that maps a specific folder as the root folder. Only files under the root folder are accessible, and not all files on your computer can be accessed directly without your permission.
The folder that maps to the root folder depends on the attributes (public, private) that you specify when initializing the FileSystem object.

The format of virtual filenames is similar to the Windows file system, except that files and folders are separated by "/" (slashes).

The virtual file name is treated as a relative path with respect to the current folder. If you specify an absolute path starting with "/", it will be treated as an absolute path from the root folder regardless of the current folder. In the initial state, the current folder points to the root folder.
The current folder can be obtained with the [PathName](/package/runtimepackage/filesystem/properties/pathname) property and can be changed with the [ChangeDir](/package/runtimepackage/filesystem/methods/changedir) method.

（Example）

（Root Folder）<br>
  ├ file1.txt          ･･･ (1)<br>
  └ folder1            ･･･ (2)<br>&ensp;
     ├ file2.txt       ･･･ (3)<br>&ensp;
     └ folder2         ･･･ (4)<br>&ensp;&ensp;;&ensp;
        └ file3.txt    ･･･ (5)<br>

        
<table>
    <tr>
        <td></td>
        <td>Current Folder</td>
        <td>Relative Path</td>
        <td>Absolute Path</td>
    </tr>
    <tr>
        <td rowspan="3">(1)</td>
        <td>/</td>
        <td>file1.txt</td>
        <td rowspan="3">/file1.txt</td>
    </tr>
    <tr>
        <td>/folder1</td>
        <td>../file1.txt</td>
    </tr>
    <tr>
        <td>/folder1/folder2</td>
        <td>../../file1.txt</td>
    </tr>
    <tr>
        <td rowspan="3">(2)</td>
        <td>/</td>
        <td>folder1</td>
        <td rowspan="3">/folder1</td>
    </tr>
    <tr>
        <td>/folder1</td>
        <td>.</td>
    </tr>
    <tr>
        <td>/folder1/folder2</td>
        <td>..</td>
    </tr>
    <tr>
        <td rowspan="3">(3)</td>
        <td>/</td>
        <td>folder1/file2.txt</td>
        <td rowspan="3">/folder1/file2.txt</td>
    </tr>
    <tr>
        <td>/folder1</td>
        <td>file2.txt</td>
    </tr>
    <tr>
        <td>/folder1/folder2</td>
        <td>../file2.txt</td>
    </tr>
    <tr>
        <td rowspan="3">(4)</td>
        <td>/</td>
        <td>folder1/folder2</td>
        <td rowspan="3">folder1/folder2</td>
    </tr>
    <tr>
        <td>/folder1</td>
        <td>folder2</td>
    </tr>
    <tr>
        <td>/folder1/folder2</td>
        <td>.</td>
    </tr>
    <tr>
        <td rowspan="3">(5)</td>
        <td>/</td>
        <td>folder1/folder2/file3.txt</td>
        <td rowspan="3">/folder1/folder2/file3.txt</td>
    </tr>
    <tr>
        <td>/folder1</td>
        <td>folder2/file3.txt</td>
    </tr>
    <tr>
        <td>/folder1/folder2</td>
        <td>file3.txt</td>
    </tr>
</table>

**Public attributes**

The FileSystem object with the public attribute specified in the [constructor](/package/runtimepackage/filesystem/methods/constructor) maps the following folders as the root folder.

| OS    |  Root folder  |
|-------|--------------------------|
| Windows Vista or later | C: \ users \ (user name) \ AppData \ Roaming \ AXIS Soft \ BizBrowser \ root |
| Windows XP<br>Windows 2000 | C: \ Documents and Settings \ (username) \ Application Data \ AXIS Soft \ BizBrowser \ root |
| Windows NT| C: \ WINNT \ Profiles \ (username) \ Application Data \ AXIS Soft \ BizBrowser \ root |
|Windows Me<br>Windows 98<br>(In case of individual user settings) | C: \ Windows \ Profiles \ (username) \ Application Data \ AXIS Soft \ BizBrowser \ root |
|Windows Me<br>Windows 98<br>(When setting common to all users) | C: \ Windows \ Application Data \ AXIS Soft \ BizBrowser \ root |
|Windows CE<br>Windows Mobile | (Installation folder) \ users \ default \ root<br>or<br>\ Windows \ Profiles \ guest \ Application Data \ AXIS Soft \ BizBrowser \ root |
| Android OS| /sdcard/Android/data/jp.co.axissoft.biz/files/filesystem/root |

<br>
**<small>Changed from "AXIS Soft" to "AXIS SOFT" (no space) since Version 5.0.0, Mobile Version 4.0.0</small>**


Folders mapped with public attributes are common to all CRS applications, so files can be shared between multiple CRS applications, but filename conflicts and illegal file content can be referenced. 

**Private attributes**

A FileSystem object with a private attribute in the [constructor](/package/runtimepackage/filesystem/methods/constructor) maps the following folders to the root folder.

| OS     | Root Folder    |
|--------|----------------|
|Windows Vista or later | C: \ users \ (user name) \ AppData \ Roaming \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
|Windows XP<br>Windows 2000 | C: \ Documents and Settings \ (username) \ Application Data \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
| Windows NT | C: \ WINNT \ Profiles \ (user name) \ Application Data \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
|Windows Me<br>Windows 98<br>(In case of individual user settings) | C: \ Windows \ Profiles \ (user name) \ Application Data \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
|Windows Me<br>Windows 98<br>(When setting common to all users) | C: \ Windows \ Application Data \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
| Windows CE<br>Windows Mobile |  (Installation folder) \ users \ default \ private_root \ (server name)<br>or<br>\ Windows \ Profiles \ guest \ Application Data \ AXIS Soft \ BizBrowser \ private_root \ (server name) |
| Android OS | /data/data/jp.co.axissoft.biz/files/filesystem/private_root/ (server name)<br>**<small>AI: This directory can only be accessed by Biz / Browser AI.</small>** |

**<small>Changed from "AXIS Soft" to "AXIS SOFT" (no space) for Version 5.0.0, Mobile Version 4.0.0</small>**

Folders that are mapped with private attributes contain the name of the server that downloaded the CRS application, so you can manage files individually for each server. It cannot be accessed from a CRS program downloaded from another server.
In addition, the FileSystem object with the private attribute can mount any folder allowed by the user with the [Mount](/package/runtimepackage/filesystem/methods/mount) method to the virtual file name.

**Access outside the root folder**

There are the following ways to access any file other than the root folder.

- Open a specific file selected by the user by the [OpenDialog](/package/runtimepackage/filesystem/methods/opendialog) method and [SaveDialog](/package/runtimepackage/filesystem/methods/savedialog) method.

- [Mount](/package/runtimepackage/filesystem/methods/mount) the folder allowed by the user with the Mount method to the virtual file name (in the case of private attribute)