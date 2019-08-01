---
title: teamsTabConfiguration リソースの種類 (オープンタイプ)
description: タブの内容を決定する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a3c16c69acefb8f746d11807a898e74de7620be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033685"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="42ffe-103">teamsTabConfiguration リソースの種類 (オープンタイプ)</span><span class="sxs-lookup"><span data-stu-id="42ffe-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="42ffe-104">[タブ](teamstab.md)の内容を決定する設定。タブが対話的に構成されている場合、この情報はタブプロバイダーアプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="42ffe-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="42ffe-105">次のプロパティに加えて、一部のタブプロバイダーアプリケーションは、追加のカスタムプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="42ffe-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="42ffe-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ffe-106">Properties</span></span>

|<span data-ttu-id="42ffe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ffe-107">Property</span></span>|<span data-ttu-id="42ffe-108">型</span><span class="sxs-lookup"><span data-stu-id="42ffe-108">Type</span></span>|<span data-ttu-id="42ffe-109">説明</span><span class="sxs-lookup"><span data-stu-id="42ffe-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="42ffe-110">entityId</span><span class="sxs-lookup"><span data-stu-id="42ffe-110">entityId</span></span>   |   <span data-ttu-id="42ffe-111">string</span><span class="sxs-lookup"><span data-stu-id="42ffe-111">string</span></span> |  <span data-ttu-id="42ffe-112">タブプロバイダによってホストされているエンティティの識別子。</span><span class="sxs-lookup"><span data-stu-id="42ffe-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="42ffe-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="42ffe-113">contentUrl</span></span> |   <span data-ttu-id="42ffe-114">string</span><span class="sxs-lookup"><span data-stu-id="42ffe-114">string</span></span> |  <span data-ttu-id="42ffe-115">Teams でのタブのコンテンツのレンダリングに使用される Url。</span><span class="sxs-lookup"><span data-stu-id="42ffe-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="42ffe-116">必須です。</span><span class="sxs-lookup"><span data-stu-id="42ffe-116">Required.</span></span>    |
|  <span data-ttu-id="42ffe-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="42ffe-117">removeUrl</span></span>  |   <span data-ttu-id="42ffe-118">string</span><span class="sxs-lookup"><span data-stu-id="42ffe-118">string</span></span> |  <span data-ttu-id="42ffe-119">Teams クライアントを使用してタブを削除したときに Teams クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="42ffe-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="42ffe-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="42ffe-120">websiteUrl</span></span> |   <span data-ttu-id="42ffe-121">string</span><span class="sxs-lookup"><span data-stu-id="42ffe-121">string</span></span> |  <span data-ttu-id="42ffe-122">Teams の外部にタブのコンテンツを表示するための Url。</span><span class="sxs-lookup"><span data-stu-id="42ffe-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="42ffe-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42ffe-123">JSON representation</span></span>

<span data-ttu-id="42ffe-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="42ffe-124">The following is a JSON representation of the resource.</span></span>
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
