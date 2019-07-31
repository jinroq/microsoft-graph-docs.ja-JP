---
author: daspek
description: itemActivity に CreateAction リソースがある場合、アクティビティがアイテムを作成したことを示します。
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e47a57e392ef629730a9de68c973d54b2ab5c2fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973182"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="0e009-103">CreateAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e009-103">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e009-104">[**itemActivity**][activity] に **CreateAction** リソースがある場合、アクティビティがアイテムを作成したことを示します。</span><span class="sxs-lookup"><span data-stu-id="0e009-104">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="0e009-105">**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0e009-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0e009-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e009-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="0e009-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e009-107">Properties</span></span>

<span data-ttu-id="0e009-108">なし。</span><span class="sxs-lookup"><span data-stu-id="0e009-108">None.</span></span> <span data-ttu-id="0e009-109">このファセットは null 値または null 以外の値になり、プロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0e009-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0e009-110">備考</span><span class="sxs-lookup"><span data-stu-id="0e009-110">Remarks</span></span>

<span data-ttu-id="0e009-111">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="0e009-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
