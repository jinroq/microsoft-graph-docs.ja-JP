---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="631ec-102">FileSystemInfo ファセット</span><span class="sxs-lookup"><span data-stu-id="631ec-102">FileSystemInfo facet</span></span>

<span data-ttu-id="631ec-103">**FileSystemInfo** リソースには、アイテムのローカル バージョンについてデバイスのローカル ファイル システムによって報告されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="631ec-103">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>
<span data-ttu-id="631ec-104">このファセットは、ローカル デバイス上でアイテムが最後に更新された日付または作成された日付を指定するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="631ec-104">The FileSystemInfo facet contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="631ec-105">これは、[driveItem][item-resource] リソースの fileSystemInfo プロパティで使用できます。</span><span class="sxs-lookup"><span data-stu-id="631ec-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="631ec-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="631ec-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="631ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="631ec-107">Properties</span></span>

| <span data-ttu-id="631ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="631ec-108">Property</span></span>                 | <span data-ttu-id="631ec-109">型</span><span class="sxs-lookup"><span data-stu-id="631ec-109">Type</span></span>           | <span data-ttu-id="631ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="631ec-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="631ec-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="631ec-111">**createdDateTime**</span></span>      | <span data-ttu-id="631ec-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631ec-112">DateTimeOffset</span></span> | <span data-ttu-id="631ec-113">クライアントでのファイルの作成日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="631ec-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="631ec-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="631ec-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="631ec-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631ec-115">DateTimeOffset</span></span> | <span data-ttu-id="631ec-116">ファイルに最後にアクセスした日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="631ec-116">The UTC date and time the file was last accessed on a client.</span></span> <span data-ttu-id="631ec-117">[最近使用したファイル一覧](../api/drive_recent.md)でのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="631ec-117">Available for the [recent file list](../api/drive_recent.md) only.</span></span> |
| <span data-ttu-id="631ec-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="631ec-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="631ec-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631ec-119">DateTimeOffset</span></span> | <span data-ttu-id="631ec-120">クライアントでファイルを最後に変更した日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="631ec-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="631ec-121">メモ</span><span class="sxs-lookup"><span data-stu-id="631ec-121">Notes</span></span>

<span data-ttu-id="631ec-122">**createdDateTime** と **lastModifiedDateTime** の値は、[DriveItem](driveitem.md) リソースの同じプロパティとは異なります。</span><span class="sxs-lookup"><span data-stu-id="631ec-122">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource.</span></span>
<span data-ttu-id="631ec-123">DriveItem リソースの値は、サービスにより認識された作成日時と更新日時です。</span><span class="sxs-lookup"><span data-stu-id="631ec-123">The properties on the driveItem resource are the created and modified date and time from the perspective of when the service saw the file.</span></span>
<span data-ttu-id="631ec-124">**FileSystemInfo** リソースに格納される値は、クライアントから提供されます。</span><span class="sxs-lookup"><span data-stu-id="631ec-124">The values stored in the **FileSystemInfo** facet are provided by the client are are the values displayed to the user if they exist.</span></span>

<span data-ttu-id="631ec-125">たとえば、あるファイルはデバイス上で月曜日に作成されたものの、火曜日までサービスにアップロードされなかった場合、ファイルをアップロードするクライアントは、`fileSystemInfo` ファセットに作成日である月曜日が含まれるように書き込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="631ec-125">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the  facet will show the original created date on Monday.</span></span> <span data-ttu-id="631ec-126">アイテムのメタデータを取得すると、アイテムの作成日は火曜日であると表示されますが、`fileSystemInfo` ファセットには元の作成日である月曜日が表示されます。</span><span class="sxs-lookup"><span data-stu-id="631ec-126">When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="631ec-p105">これらのプロパティは編集可能です。ファイルをアップロードして、これらのフィールドのローカル クライアントを知っている場合は、その値を要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="631ec-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="631ec-129">ファイルの内容を更新し、これらのプロパティが指定されていない場合、**lastModifiedDateTime** は自動的に現在の時刻にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="631ec-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="631ec-130">備考</span><span class="sxs-lookup"><span data-stu-id="631ec-130">Remarks</span></span>

* <span data-ttu-id="631ec-131">**lastAccessedDateTime** は、SharePoint Online または OneDrive for Business のアイテムでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="631ec-131">**lastAccessedDateTime** is not available for items in SharePoint online, OneDrive for Business, or SharePoint Server 2016.</span></span>

<span data-ttu-id="631ec-132">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="631ec-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
