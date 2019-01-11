---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a845a6609991041f12266cd97e95460f96bf742f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876763"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="71cf0-102">DeleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71cf0-102">DeleteAction resource type</span></span>

> <span data-ttu-id="71cf0-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71cf0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71cf0-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71cf0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71cf0-105">[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="71cf0-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="71cf0-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71cf0-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="71cf0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71cf0-107">Properties</span></span>

| <span data-ttu-id="71cf0-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="71cf0-108">Property name</span></span> | <span data-ttu-id="71cf0-109">Type</span><span class="sxs-lookup"><span data-stu-id="71cf0-109">Type</span></span>   | <span data-ttu-id="71cf0-110">説明</span><span class="sxs-lookup"><span data-stu-id="71cf0-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="71cf0-111">name</span><span class="sxs-lookup"><span data-stu-id="71cf0-111">name</span></span>          | <span data-ttu-id="71cf0-112">文字列</span><span class="sxs-lookup"><span data-stu-id="71cf0-112">string</span></span> | <span data-ttu-id="71cf0-113">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="71cf0-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="71cf0-114">objectType</span><span class="sxs-lookup"><span data-stu-id="71cf0-114">objectType</span></span>    | <span data-ttu-id="71cf0-115">文字列</span><span class="sxs-lookup"><span data-stu-id="71cf0-115">string</span></span> | <span data-ttu-id="71cf0-116">`File`または`Folder`に削除された項目の種類に依存します。</span><span class="sxs-lookup"><span data-stu-id="71cf0-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="71cf0-117">備考</span><span class="sxs-lookup"><span data-stu-id="71cf0-117">Remarks</span></span>

<span data-ttu-id="71cf0-118">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="71cf0-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
