---
title: teamsTabConfiguration リソースの種類 (オープン型)
description: タブの内容を決定する設定です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10cc22e70288d1643a3a2cdebe23a012e22e3879
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519200"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="26a57-103">teamsTabConfiguration リソースの種類 (オープン型)</span><span class="sxs-lookup"><span data-stu-id="26a57-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a57-104">[タブ](teamstab.md)の内容を決定する設定です。タブが対話形式で構成されている場合、この情報は、タブ プロバイダー アプリケーションによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="26a57-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="26a57-105">に加えて、以下のプロパティは、タブ プロバイダー アプリケーションをいくつかは、追加のカスタム プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="26a57-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="26a57-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26a57-106">Properties</span></span>

|<span data-ttu-id="26a57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26a57-107">Property</span></span>|<span data-ttu-id="26a57-108">型</span><span class="sxs-lookup"><span data-stu-id="26a57-108">Type</span></span>|<span data-ttu-id="26a57-109">説明</span><span class="sxs-lookup"><span data-stu-id="26a57-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="26a57-110">entityId</span><span class="sxs-lookup"><span data-stu-id="26a57-110">entityId</span></span>   |   <span data-ttu-id="26a57-111">string</span><span class="sxs-lookup"><span data-stu-id="26a57-111">string</span></span> |  <span data-ttu-id="26a57-112">タブ プロバイダーによってホストされているエンティティの識別子です。</span><span class="sxs-lookup"><span data-stu-id="26a57-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="26a57-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="26a57-113">contentUrl</span></span> |   <span data-ttu-id="26a57-114">string</span><span class="sxs-lookup"><span data-stu-id="26a57-114">string</span></span> |  <span data-ttu-id="26a57-115">チームでのタブの内容を表示するために使用される Url です。</span><span class="sxs-lookup"><span data-stu-id="26a57-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="26a57-116">必須です。</span><span class="sxs-lookup"><span data-stu-id="26a57-116">Required.</span></span>    |
|  <span data-ttu-id="26a57-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="26a57-117">removeUrl</span></span>  |   <span data-ttu-id="26a57-118">string</span><span class="sxs-lookup"><span data-stu-id="26a57-118">string</span></span> |  <span data-ttu-id="26a57-119">チームのクライアントを使用してタブが削除されたときに、チーム クライアントによって呼び出される Url。</span><span class="sxs-lookup"><span data-stu-id="26a57-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="26a57-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="26a57-120">websiteUrl</span></span> |   <span data-ttu-id="26a57-121">文字列</span><span class="sxs-lookup"><span data-stu-id="26a57-121">string</span></span> |  <span data-ttu-id="26a57-122">チーム以外のタブの内容を表示するための Url です。</span><span class="sxs-lookup"><span data-stu-id="26a57-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="26a57-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26a57-123">JSON representation</span></span>

<span data-ttu-id="26a57-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26a57-124">The following is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
