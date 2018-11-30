---
title: teamsTabConfiguration リソースの種類 (オープン型)
description: タブの内容を決定する設定です。
ms.openlocfilehash: 4d04ca9128760ee6fed9c0fa704fa991384ac17a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020453"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="1d8eb-103">teamsTabConfiguration リソースの種類 (オープン型)</span><span class="sxs-lookup"><span data-stu-id="1d8eb-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="1d8eb-104">[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="1d8eb-105">に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="1d8eb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d8eb-106">Properties</span></span>

|<span data-ttu-id="1d8eb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d8eb-107">Property</span></span>|<span data-ttu-id="1d8eb-108">型</span><span class="sxs-lookup"><span data-stu-id="1d8eb-108">Type</span></span>|<span data-ttu-id="1d8eb-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d8eb-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="1d8eb-110">エンティティ Id</span><span class="sxs-lookup"><span data-stu-id="1d8eb-110">entityId</span></span>   |   <span data-ttu-id="1d8eb-111">文字列</span><span class="sxs-lookup"><span data-stu-id="1d8eb-111">string</span></span> |  <span data-ttu-id="1d8eb-112">タブ プロバイダーによってホストされているエンティティの識別子です。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="1d8eb-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="1d8eb-113">contentUrl</span></span> |   <span data-ttu-id="1d8eb-114">文字列</span><span class="sxs-lookup"><span data-stu-id="1d8eb-114">string</span></span> |  <span data-ttu-id="1d8eb-115">チームでのタブの内容を表示するために使用される Url です。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="1d8eb-116">必須。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-116">Required.</span></span>    |
|  <span data-ttu-id="1d8eb-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="1d8eb-117">removeUrl</span></span>  |   <span data-ttu-id="1d8eb-118">文字列</span><span class="sxs-lookup"><span data-stu-id="1d8eb-118">string</span></span> |  <span data-ttu-id="1d8eb-119">チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="1d8eb-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="1d8eb-120">websiteUrl</span></span> |   <span data-ttu-id="1d8eb-121">文字列</span><span class="sxs-lookup"><span data-stu-id="1d8eb-121">string</span></span> |  <span data-ttu-id="1d8eb-122">チーム以外のタブの内容を表示するための Url です。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="1d8eb-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d8eb-123">JSON representation</span></span>

<span data-ttu-id="1d8eb-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d8eb-124">The following is a JSON representation of the resource.</span></span>
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
