# FileZip

FileZip creates password-protected ZIP and 7z archives directly from Finder.

- Works offline
- No additional software required
- Supports macOS 13 Ventura and later
- About 7 MB installed
- About 3 MB download

Source code and releases are available at [github.com/dwdas9/FileZip](https://github.com/dwdas9/FileZip).

---

## 1. Download FileZip

[**Download FileZip 1.0.0**](https://github.com/dwdas9/FileZip/releases/download/v1.0.0/FileZip-1.0.0.dmg)

If Safari asks for permission to download from GitHub, click **Allow**.

You can also download it from the [FileZip releases page](https://github.com/dwdas9/FileZip/releases/tag/v1.0.0). Under **Assets**, select **FileZip-1.0.0.dmg**.

---

## 2. Install FileZip

1. Open **FileZip-1.0.0.dmg**.
2. Drag **FileZip** into the **Applications** folder.
3. Eject the FileZip disk image.
4. Open FileZip from **Applications**.

<img src="images/install-dmg.png" width="600" alt="FileZip installer showing the FileZip app and Applications folder">

*Drag FileZip into Applications.*

You can delete the DMG after installation.

### If macOS blocks FileZip

macOS may block FileZip the first time you open it because the app is not notarised by Apple.

1. Close the warning.
2. Open **System Settings > Privacy & Security**.
3. Find the message about FileZip and click **Open Anyway**.
4. Confirm when prompted.

You only need to do this once. There is no need to disable any macOS security settings.

---

## 3. Enable Finder Quick Actions

Open FileZip and click **Install Quick Actions**.

<img src="images/home.png" width="460" alt="FileZip showing Finder Quick Actions as installed">

Once installed, FileZip adds these options to Finder:

- **Compress with Password**
- **Extract with FileZip**

If they do not appear immediately, restart Finder or your Mac.

---

## 4. Create a password-protected archive

1. Select one or more files or folders in Finder.
2. Right-click the selection.
3. Choose **Quick Actions > Compress with Password**.
4. Choose the archive name, location and format.
5. Enter and confirm the password.
6. Click **Compress**.

<img src="images/compress.png" width="500" alt="Compress with Password window showing archive name, location, ZIP format and password fields">

<img src="images/compressing.png" width="500" alt="FileZip compression progress">

<img src="images/compressed.png" width="500" alt="FileZip showing that the encrypted archive was created successfully">

The archive is created as a new file. Your original files are not changed.

You can also start by dragging files onto the FileZip window or its Dock icon.

### ZIP or 7z?

**ZIP** is the best choice for most cases. It is supported by more applications. File names inside the archive remain visible, but the contents are encrypted.

**7z** also encrypts the file names and supports a wider range of password characters. The recipient will need an application that supports 7z, such as 7-Zip, Keka or The Unarchiver.

Keep your password somewhere safe. FileZip cannot recover a forgotten password.

---

## 5. Extract an archive

1. Right-click the archive in Finder.
2. Choose **Quick Actions > Extract with FileZip**.
3. Enter the password.
4. Click **Extract**.

You can also drag the archive onto FileZip.

<img src="images/extract.png" width="480" alt="FileZip Extract window with password and destination fields">

<img src="images/extracted.png" width="480" alt="FileZip showing a completed extraction">

FileZip does not overwrite existing files. If a file or folder with the same name already exists, FileZip gives the extracted copy a new name, such as **Project Files 2** or **Report 2.pdf**.

### Opening encrypted ZIP files in Finder

The built-in macOS Archive Utility may fail to open ZIP files created with FileZip.

If that happens, use **Extract with FileZip** instead.

---

## 6. Share an archive

Send the archive by email, messaging app, cloud storage, USB drive or any other method you normally use.

For sensitive files, send the password separately from the archive.

Other applications that can open these archives include:

- **Windows:** 7-Zip
- **macOS:** Keka or The Unarchiver

Mac users can also install FileZip.

---

## Troubleshooting

### FileZip asks for access to Desktop, Documents or Downloads

Click **Allow**. macOS requires this permission before FileZip can read or save files in those locations.

FileZip works locally and does not upload your files.

### The password is incorrect

Passwords are case-sensitive. Check the password and make sure Caps Lock is not on.

<img src="images/wrong-password.png" width="480" alt="FileZip showing an incorrect password message">

### Quick Actions are missing

Open FileZip and make sure **Install Quick Actions** has been completed.

You can also check:

**Right-click a file > Quick Actions > Customize...**

If the actions are enabled but still do not appear, restart Finder or your Mac.

### How do I cancel an operation?

Click **Cancel**. Incomplete output is removed automatically.

### Does FileZip support RAR?

No. FileZip supports ZIP, 7z, TAR, GZ, BZ2 and XZ.

---

## Remove FileZip

1. Open FileZip and click **Remove** under Quick Actions.
2. Quit FileZip.
3. Move FileZip from **Applications** to the Trash.

Removing FileZip does not affect archives you have already created.

---

FileZip uses **7-Zip**, created by Igor Pavlov.

See [Third-Party Notices](THIRD_PARTY_NOTICES.md) for licensing information.