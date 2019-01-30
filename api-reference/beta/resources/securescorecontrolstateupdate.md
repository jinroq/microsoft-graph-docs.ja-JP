---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641730"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="5008d-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5008d-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="5008d-104">ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。</span><span class="sxs-lookup"><span data-stu-id="5008d-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="5008d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5008d-105">Property</span></span> |<span data-ttu-id="5008d-106">型</span><span class="sxs-lookup"><span data-stu-id="5008d-106">Type</span></span> |<span data-ttu-id="5008d-107">説明</span><span class="sxs-lookup"><span data-stu-id="5008d-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="5008d-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="5008d-108">assignedTo</span></span> | <span data-ttu-id="5008d-109">string</span><span class="sxs-lookup"><span data-stu-id="5008d-109">string</span></span> | <span data-ttu-id="5008d-110">処理はユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="5008d-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="5008d-111">comment</span><span class="sxs-lookup"><span data-stu-id="5008d-111">comment</span></span> | <span data-ttu-id="5008d-112">string</span><span class="sxs-lookup"><span data-stu-id="5008d-112">string</span></span> | <span data-ttu-id="5008d-113">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="5008d-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="5008d-114">state</span><span class="sxs-lookup"><span data-stu-id="5008d-114">state</span></span> | <span data-ttu-id="5008d-115">string</span><span class="sxs-lookup"><span data-stu-id="5008d-115">string</span></span> | <span data-ttu-id="5008d-116">修正プログラムのコマンドを使用してコントロールの状態を変更することができます (Ex: 無視され、サード ・ パーティなど)</span><span class="sxs-lookup"><span data-stu-id="5008d-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="5008d-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="5008d-117">updatedBy</span></span> | <span data-ttu-id="5008d-118">string</span><span class="sxs-lookup"><span data-stu-id="5008d-118">string</span></span> |<span data-ttu-id="5008d-119">テナントの状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="5008d-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="5008d-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5008d-120">updatedDateTime</span></span> | <span data-ttu-id="5008d-121">DateTimeOffset でしょうか。</span><span class="sxs-lookup"><span data-stu-id="5008d-121">DateTimeOffset?</span></span> |<span data-ttu-id="5008d-122">コントロールの状態が更新された時間</span><span class="sxs-lookup"><span data-stu-id="5008d-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="5008d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5008d-123">JSON representation</span></span>
 <span data-ttu-id="5008d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5008d-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
