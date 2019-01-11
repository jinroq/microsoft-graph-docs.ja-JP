---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: 9a033a08b496225620245bb48cd1b0bef1f2a323
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806847"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="52bfe-102">FileSystemInfo ファセット</span><span class="sxs-lookup"><span data-stu-id="52bfe-102">FileSystemInfo facet</span></span>

<span data-ttu-id="52bfe-p101">**FileSystemInfo** リソースには、アイテムのローカル バージョンについてデバイスのローカル ファイル システムによって報告されるプロパティが含まれています。このファセットは、ローカル デバイス上で、アイテムが最後に更新または作成された日付を指定するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="52bfe-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="52bfe-105">これは、[driveItem][item-resource] リソースの fileSystemInfo プロパティで使用できます。</span><span class="sxs-lookup"><span data-stu-id="52bfe-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52bfe-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52bfe-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="52bfe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52bfe-107">Properties</span></span>

| <span data-ttu-id="52bfe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52bfe-108">Property</span></span>                 | <span data-ttu-id="52bfe-109">型</span><span class="sxs-lookup"><span data-stu-id="52bfe-109">Type</span></span>           | <span data-ttu-id="52bfe-110">説明</span><span class="sxs-lookup"><span data-stu-id="52bfe-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="52bfe-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="52bfe-111">**createdDateTime**</span></span>      | <span data-ttu-id="52bfe-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52bfe-112">DateTimeOffset</span></span> | <span data-ttu-id="52bfe-113">クライアントでのファイルの作成日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="52bfe-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="52bfe-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="52bfe-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="52bfe-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52bfe-115">DateTimeOffset</span></span> | <span data-ttu-id="52bfe-p102">ファイルに最後にアクセスした日時 (UTC)。[最近使用したファイル一覧](../api/drive-recent.md)でのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="52bfe-p102">The UTC date and time the file was last accessed. Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="52bfe-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="52bfe-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="52bfe-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52bfe-119">DateTimeOffset</span></span> | <span data-ttu-id="52bfe-120">クライアントでファイルを最後に変更した日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="52bfe-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="52bfe-121">メモ</span><span class="sxs-lookup"><span data-stu-id="52bfe-121">Notes</span></span>

<span data-ttu-id="52bfe-p103">**createdDateTime** と **lastModifiedDateTime** の値は、[DriveItem](driveitem.md) リソースの同じプロパティとは異なります。DriveItem リソースの値は、サービスにより認識された作成日時と更新日時です。**FileSystemInfo** リソースで保存されている値は、クライアントによって指定されています。</span><span class="sxs-lookup"><span data-stu-id="52bfe-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="52bfe-p104">たとえば、ファイルがデバイス上で月曜日に作成されたものの、火曜日までアップロードされなかった場合、ファイルをアップロードするクライアントは、`fileSystemInfo` ファセットに作成日である月曜日が含まれるように書き込む必要があります。アイテムのメタデータを取得すると、アイテムの作成日には火曜日が示されますが、`fileSystemInfo` ファセットには元の作成日である月曜日が表示されます。</span><span class="sxs-lookup"><span data-stu-id="52bfe-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="52bfe-p105">これらのプロパティは編集可能です。ファイルをアップロードして、これらのフィールドのローカル クライアントを知っている場合は、その値を要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="52bfe-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="52bfe-129">ファイルの内容を更新し、これらのプロパティが指定されていない場合、**lastModifiedDateTime** は自動的に現在の時刻にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="52bfe-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="52bfe-130">備考</span><span class="sxs-lookup"><span data-stu-id="52bfe-130">Remarks</span></span>

* <span data-ttu-id="52bfe-131">**lastAccessedDateTime** は、SharePoint Online または OneDrive for Business のアイテムには使用できません。</span><span class="sxs-lookup"><span data-stu-id="52bfe-131">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="52bfe-132">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52bfe-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
