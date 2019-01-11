---
title: teamsTabConfiguration リソースの種類 (オープン型)
description: タブの内容を決定する設定です。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c33ab6d5102498ab26fcc609328c2562707883d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858472"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="d3900-103">teamsTabConfiguration リソースの種類 (オープン型)</span><span class="sxs-lookup"><span data-stu-id="d3900-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="d3900-104">[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="d3900-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="d3900-105">に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="d3900-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="d3900-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3900-106">Properties</span></span>

|<span data-ttu-id="d3900-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3900-107">Property</span></span>|<span data-ttu-id="d3900-108">種類</span><span class="sxs-lookup"><span data-stu-id="d3900-108">Type</span></span>|<span data-ttu-id="d3900-109">説明</span><span class="sxs-lookup"><span data-stu-id="d3900-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="d3900-110">entityId</span><span class="sxs-lookup"><span data-stu-id="d3900-110">entityId</span></span>   |   <span data-ttu-id="d3900-111">文字列</span><span class="sxs-lookup"><span data-stu-id="d3900-111">string</span></span> |  <span data-ttu-id="d3900-112">タブ プロバイダーによってホストされているエンティティの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d3900-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="d3900-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d3900-113">contentUrl</span></span> |   <span data-ttu-id="d3900-114">文字列</span><span class="sxs-lookup"><span data-stu-id="d3900-114">string</span></span> |  <span data-ttu-id="d3900-115">チームでのタブの内容を表示するために使用される Url です。</span><span class="sxs-lookup"><span data-stu-id="d3900-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="d3900-116">必須。</span><span class="sxs-lookup"><span data-stu-id="d3900-116">Required.</span></span>    |
|  <span data-ttu-id="d3900-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="d3900-117">removeUrl</span></span>  |   <span data-ttu-id="d3900-118">文字列</span><span class="sxs-lookup"><span data-stu-id="d3900-118">string</span></span> |  <span data-ttu-id="d3900-119">チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="d3900-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="d3900-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="d3900-120">websiteUrl</span></span> |   <span data-ttu-id="d3900-121">文字列</span><span class="sxs-lookup"><span data-stu-id="d3900-121">string</span></span> |  <span data-ttu-id="d3900-122">チーム以外のタブの内容を表示するための Url です。</span><span class="sxs-lookup"><span data-stu-id="d3900-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="d3900-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3900-123">JSON representation</span></span>

<span data-ttu-id="d3900-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3900-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
