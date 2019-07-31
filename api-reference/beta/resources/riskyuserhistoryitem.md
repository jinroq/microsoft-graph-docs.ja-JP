---
title: riskyUserHistoryItem リソースの種類
description: Azure AD ユーザーのリスク履歴を表します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 586fdb046adc8977550cc386a27284752cf487c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965335"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="d912b-103">riskyUserHistoryItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d912b-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="d912b-104">Azure ad Id 保護によって決定された Azure AD ユーザーのリスク履歴を表します。</span><span class="sxs-lookup"><span data-stu-id="d912b-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="d912b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d912b-105">Methods</span></span>

| <span data-ttu-id="d912b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d912b-106">Method</span></span>   | <span data-ttu-id="d912b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d912b-107">Return Type</span></span>|<span data-ttu-id="d912b-108">説明</span><span class="sxs-lookup"><span data-stu-id="d912b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d912b-109">リストの履歴</span><span class="sxs-lookup"><span data-stu-id="d912b-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="d912b-110">[riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d912b-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="d912b-111">Azure AD ユーザーのリスク履歴を取得します。</span><span class="sxs-lookup"><span data-stu-id="d912b-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="d912b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d912b-112">Properties</span></span>

| <span data-ttu-id="d912b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d912b-113">Property</span></span>       | <span data-ttu-id="d912b-114">型</span><span class="sxs-lookup"><span data-stu-id="d912b-114">Type</span></span>    | <span data-ttu-id="d912b-115">説明</span><span class="sxs-lookup"><span data-stu-id="d912b-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="d912b-116">userId</span><span class="sxs-lookup"><span data-stu-id="d912b-116">userId</span></span>         | <span data-ttu-id="d912b-117">string</span><span class="sxs-lookup"><span data-stu-id="d912b-117">string</span></span>  | <span data-ttu-id="d912b-118">ユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="d912b-118">The id of the user.</span></span> |
| <span data-ttu-id="d912b-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d912b-119">initiatedBy</span></span>    | <span data-ttu-id="d912b-120">bool</span><span class="sxs-lookup"><span data-stu-id="d912b-120">bool</span></span>    | <span data-ttu-id="d912b-121">操作を実行するアクターの id。</span><span class="sxs-lookup"><span data-stu-id="d912b-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="d912b-122">activity</span><span class="sxs-lookup"><span data-stu-id="d912b-122">activity</span></span>       | [<span data-ttu-id="d912b-123">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="d912b-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="d912b-124">ユーザーのリスクレベルの変更に関連するアクティビティ。</span><span class="sxs-lookup"><span data-stu-id="d912b-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="d912b-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d912b-125">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
