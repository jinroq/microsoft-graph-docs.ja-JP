---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 08a79a265e8d4dbda3017a1ff8a32c5e4cab51ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067186"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="88c88-102">FileSystemInfo ファセット</span><span class="sxs-lookup"><span data-stu-id="88c88-102">FileSystemInfo facet</span></span>

> <span data-ttu-id="88c88-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="88c88-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88c88-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88c88-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88c88-p102">**FileSystemInfo** リソースには、アイテムのローカル バージョンについてデバイスのローカル ファイル システムによって報告されるプロパティが含まれています。このファセットは、ローカル デバイス上で、アイテムが最後に更新または作成された日付を指定するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="88c88-p102">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="88c88-107">これは、[driveItem][item-resource] リソースの fileSystemInfo プロパティで使用できます。</span><span class="sxs-lookup"><span data-stu-id="88c88-107">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88c88-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88c88-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="88c88-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88c88-109">Properties</span></span>

| <span data-ttu-id="88c88-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88c88-110">Property</span></span>                 | <span data-ttu-id="88c88-111">型</span><span class="sxs-lookup"><span data-stu-id="88c88-111">Type</span></span>           | <span data-ttu-id="88c88-112">説明</span><span class="sxs-lookup"><span data-stu-id="88c88-112">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="88c88-113">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="88c88-113">**createdDateTime**</span></span>      | <span data-ttu-id="88c88-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c88-114">DateTimeOffset</span></span> | <span data-ttu-id="88c88-115">クライアントでのファイルの作成日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="88c88-115">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="88c88-116">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="88c88-116">**lastAccessedDateTime**</span></span> | <span data-ttu-id="88c88-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c88-117">DateTimeOffset</span></span> | <span data-ttu-id="88c88-p103">ファイルに最後にアクセスした日時 (UTC)。[最近使用したファイル一覧](../api/drive-recent.md)でのみ使用可能です。</span><span class="sxs-lookup"><span data-stu-id="88c88-p103">The UTC date and time the file was last accessed. Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="88c88-120">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="88c88-120">**lastModifiedDateTime**</span></span> | <span data-ttu-id="88c88-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c88-121">DateTimeOffset</span></span> | <span data-ttu-id="88c88-122">クライアントでファイルを最後に変更した日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="88c88-122">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="88c88-123">メモ</span><span class="sxs-lookup"><span data-stu-id="88c88-123">Notes</span></span>

<span data-ttu-id="88c88-p104">**createdDateTime** と **lastModifiedDateTime** の値は、[DriveItem](driveitem.md) リソースの同じプロパティとは異なります。DriveItem リソースの値は、サービスにより認識された作成日時と更新日時です。**FileSystemInfo** リソースで保存されている値は、クライアントによって指定されています。</span><span class="sxs-lookup"><span data-stu-id="88c88-p104">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="88c88-p105">たとえば、ファイルがデバイス上で月曜日に作成されたものの、火曜日までアップロードされなかった場合、ファイルをアップロードするクライアントは、`fileSystemInfo` ファセットに作成日である月曜日が含まれるように書き込む必要があります。アイテムのメタデータを取得すると、アイテムの作成日には火曜日が示されますが、`fileSystemInfo` ファセットには元の作成日である月曜日が表示されます。</span><span class="sxs-lookup"><span data-stu-id="88c88-p105">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="88c88-p106">これらのプロパティは編集可能です。ファイルをアップロードして、これらのフィールドのローカル クライアントを知っている場合は、その値を要求に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="88c88-p106">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="88c88-131">ファイルの内容を更新し、これらのプロパティが指定されていない場合、**lastModifiedDateTime** は自動的に現在の時刻にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="88c88-131">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="88c88-132">備考</span><span class="sxs-lookup"><span data-stu-id="88c88-132">Remarks</span></span>

* <span data-ttu-id="88c88-133">**lastAccessedDateTime** は、SharePoint Online または OneDrive for Business のアイテムでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="88c88-133">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="88c88-134">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88c88-134">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
