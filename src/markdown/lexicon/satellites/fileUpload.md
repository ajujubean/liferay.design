---
title: "File Upload"
titleLabel: "Portal"
description: "File Uploader is a pattern that lets users select and upload images to the system."
layout: "guide"
order: 1
---

<div class="page-description">File Uploader is a pattern that lets users select and upload images to the system.</div>

### Simple File Upload
Simple file upload is used to upload a simple file element.

![file upload simple](/lexicon/images/FileUploadSimple.png)

### Multiple File Upload
Inside this categorization we have two different patterns: file uploader and image uploader. Both are pretty similar, but the second one is more visual and adapted to the situation.

Both uploaders share the same **upload area** which has the following attributes:
* It must always have two different states:
    * Default
        * Message: clarifies the permitted file extensions and max size of each file
        * Secondary button: users may not always want to use the drag and drop feature. The button opens the operating system's file uploader with the option to select multiple files.

        ![file upload simple empty state](/lexicon/images/FileUploadEmptyState.png)

    * Active
        * It contains an animation that invites users to drop documents on dropover state.

        ![file upload simple empty state hover](/lexicon/images/FileUploadEmptyStateHover.png)

* Once files have been added to the upload system, there must be clear options to upload more files: An explicit button and a drag and drop option.
* The scroll must only be vertical if needed.
* Each file can be deleted individually.
* Each file can retry the upload individually.

#### File Uploader

![file upload simple](/lexicon/images/FileUpload.png)

* File uploader accepts any file, including images, pdfs, docs, etc.
* After dropping files in the area, the upload status of each file is displayed in a list.
* Files that didn't complete the upload process provide the option to retry the upload.
* Every file must be removable.

In this example, the file uploader works together with a form to predefine configuration options for the uploaded files:

![file upload simple with errors](/lexicon/images/FileUploaderErrorStatePanelOpen.png)

Files can be in different states:

* Default state: when the file is already uploaded

![file upload list row default state](/lexicon/images/FileUploadListDefault.png)

* Upload state: during the upload process

![file upload list row upload state](/lexicon/images/FileUploadListProgress.png)

* Error state: when the file upload has failed

![file upload list row error state](/lexicon/images/FileUploadListError.png)


#### Image Uploader

![file upload simple](/lexicon/images/FileUploadImageUpload.png)

* Image uploader only admits image file types.
* After dropping images in the area, an image grid appears, letting the user see the upload process.
* The drag and drop area fills the image grid. This area must have a vertical scroll. The cell next to the last uploaded image must have a "+" to invite the user to upload more files. Clicking in that cell opens the file upload for the specified files.
* Each image is represented by a square thumbnail.
* Images that didn't complete the upload process provide the option to retry the upload.
* Every image must be removable.

![image upload with error state](/lexicon/images/FileUploadImageUploadErrors.png)

Images can be in different states:

* Upload state: during the upload process. The default state is shown in the image on the left. The hover state is shown in the image on the right.

![image upload, upload state](/lexicon/images/FileUploadImageStates.png)

* Error state: when the file upload has failed

![image upload error state](/lexicon/images/FileUploadImageStatesError.png)

* Default and hover image states: when the file is already uploaded

![image default and hover state](/lexicon/images/FileUploadImageStatesDefaultHover.png)

* The image uploader may require a checked state for certain options:

![image default and selected state](/lexicon/images/FileUploadImageStatesChecbox.png)