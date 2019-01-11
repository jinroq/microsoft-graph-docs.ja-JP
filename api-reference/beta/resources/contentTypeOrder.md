---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ad25ececa9a32a1aaab7f25bf909f7e1ef640dec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825754"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="0c334-102">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c334-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="0c334-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c334-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c334-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c334-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c334-105">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c334-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c334-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c334-106">JSON representation</span></span>

<span data-ttu-id="0c334-107">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c334-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="0c334-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c334-108">Properties</span></span>

| <span data-ttu-id="0c334-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0c334-109">Property name</span></span> | <span data-ttu-id="0c334-110">Type</span><span class="sxs-lookup"><span data-stu-id="0c334-110">Type</span></span>    | <span data-ttu-id="0c334-111">説明</span><span class="sxs-lookup"><span data-stu-id="0c334-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="0c334-112">**default**</span><span class="sxs-lookup"><span data-stu-id="0c334-112">**default**</span></span>   | <span data-ttu-id="0c334-113">boolean</span><span class="sxs-lookup"><span data-stu-id="0c334-113">boolean</span></span> | <span data-ttu-id="0c334-114">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="0c334-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="0c334-115">**position**</span><span class="sxs-lookup"><span data-stu-id="0c334-115">**position**</span></span>  | <span data-ttu-id="0c334-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0c334-116">Int32</span></span>   | <span data-ttu-id="0c334-117">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c334-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
