---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068983"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="90fb7-102">DeleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90fb7-102">DeleteAction resource type</span></span>

> <span data-ttu-id="90fb7-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90fb7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90fb7-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90fb7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90fb7-105">[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="90fb7-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="90fb7-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90fb7-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="90fb7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90fb7-107">Properties</span></span>

| <span data-ttu-id="90fb7-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="90fb7-108">Property name</span></span> | <span data-ttu-id="90fb7-109">型</span><span class="sxs-lookup"><span data-stu-id="90fb7-109">Type</span></span>   | <span data-ttu-id="90fb7-110">説明</span><span class="sxs-lookup"><span data-stu-id="90fb7-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="90fb7-111">name</span><span class="sxs-lookup"><span data-stu-id="90fb7-111">name</span></span>          | <span data-ttu-id="90fb7-112">文字列</span><span class="sxs-lookup"><span data-stu-id="90fb7-112">string</span></span> | <span data-ttu-id="90fb7-113">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="90fb7-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="90fb7-114">objectType</span><span class="sxs-lookup"><span data-stu-id="90fb7-114">objectType</span></span>    | <span data-ttu-id="90fb7-115">文字列</span><span class="sxs-lookup"><span data-stu-id="90fb7-115">string</span></span> | <span data-ttu-id="90fb7-116">`File`または`Folder`に削除された項目の種類に依存します。</span><span class="sxs-lookup"><span data-stu-id="90fb7-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="90fb7-117">備考</span><span class="sxs-lookup"><span data-stu-id="90fb7-117">Remarks</span></span>

<span data-ttu-id="90fb7-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="90fb7-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
