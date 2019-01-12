---
title: teamsTabConfiguration リソースの種類 (オープン型)
description: タブの内容を決定する設定です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 515e5896591b58054f161ff740f68b0ca4913663
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913486"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="a6bad-103">teamsTabConfiguration リソースの種類 (オープン型)</span><span class="sxs-lookup"><span data-stu-id="a6bad-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="a6bad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6bad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6bad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6bad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6bad-106">[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="a6bad-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="a6bad-107">に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="a6bad-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="a6bad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6bad-108">Properties</span></span>

|<span data-ttu-id="a6bad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6bad-109">Property</span></span>|<span data-ttu-id="a6bad-110">種類</span><span class="sxs-lookup"><span data-stu-id="a6bad-110">Type</span></span>|<span data-ttu-id="a6bad-111">説明</span><span class="sxs-lookup"><span data-stu-id="a6bad-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="a6bad-112">entityId</span><span class="sxs-lookup"><span data-stu-id="a6bad-112">entityId</span></span>   |   <span data-ttu-id="a6bad-113">文字列</span><span class="sxs-lookup"><span data-stu-id="a6bad-113">string</span></span> |  <span data-ttu-id="a6bad-114">タブ プロバイダーによってホストされているエンティティの識別子です。</span><span class="sxs-lookup"><span data-stu-id="a6bad-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="a6bad-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a6bad-115">contentUrl</span></span> |   <span data-ttu-id="a6bad-116">文字列</span><span class="sxs-lookup"><span data-stu-id="a6bad-116">string</span></span> |  <span data-ttu-id="a6bad-117">チームでのタブの内容を表示するために使用される Url です。</span><span class="sxs-lookup"><span data-stu-id="a6bad-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="a6bad-118">必須。</span><span class="sxs-lookup"><span data-stu-id="a6bad-118">Required.</span></span>    |
|  <span data-ttu-id="a6bad-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="a6bad-119">removeUrl</span></span>  |   <span data-ttu-id="a6bad-120">文字列</span><span class="sxs-lookup"><span data-stu-id="a6bad-120">string</span></span> |  <span data-ttu-id="a6bad-121">チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="a6bad-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="a6bad-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="a6bad-122">websiteUrl</span></span> |   <span data-ttu-id="a6bad-123">文字列</span><span class="sxs-lookup"><span data-stu-id="a6bad-123">string</span></span> |  <span data-ttu-id="a6bad-124">チーム以外のタブの内容を表示するための Url です。</span><span class="sxs-lookup"><span data-stu-id="a6bad-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="a6bad-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6bad-125">JSON representation</span></span>

<span data-ttu-id="a6bad-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6bad-126">The following is a JSON representation of the resource.</span></span>
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
