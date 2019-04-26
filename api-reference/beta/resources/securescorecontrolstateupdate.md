---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、Default、ThirdParty、、レビュー済み) があります。
localization_priority: Normal
ms.openlocfilehash: 24febeb4bfb055e89e59cdb4f79c8b60c6c40347
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343361"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="8bdfa-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bdfa-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="8bdfa-104">ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。</span><span class="sxs-lookup"><span data-stu-id="8bdfa-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="8bdfa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bdfa-105">Property</span></span> |<span data-ttu-id="8bdfa-106">型</span><span class="sxs-lookup"><span data-stu-id="8bdfa-106">Type</span></span> |<span data-ttu-id="8bdfa-107">説明</span><span class="sxs-lookup"><span data-stu-id="8bdfa-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="8bdfa-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="8bdfa-108">assignedTo</span></span> | <span data-ttu-id="8bdfa-109">string</span><span class="sxs-lookup"><span data-stu-id="8bdfa-109">string</span></span> | <span data-ttu-id="8bdfa-110">アクションを実行するユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="8bdfa-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="8bdfa-111">comment</span><span class="sxs-lookup"><span data-stu-id="8bdfa-111">comment</span></span> | <span data-ttu-id="8bdfa-112">string</span><span class="sxs-lookup"><span data-stu-id="8bdfa-112">string</span></span> | <span data-ttu-id="8bdfa-113">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="8bdfa-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="8bdfa-114">state</span><span class="sxs-lookup"><span data-stu-id="8bdfa-114">state</span></span> | <span data-ttu-id="8bdfa-115">string</span><span class="sxs-lookup"><span data-stu-id="8bdfa-115">string</span></span> | <span data-ttu-id="8bdfa-116">PATCH コマンドを使用してコントロールの状態を変更できます (例: 無視、thirdParty など)</span><span class="sxs-lookup"><span data-stu-id="8bdfa-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="8bdfa-117">updatedby</span><span class="sxs-lookup"><span data-stu-id="8bdfa-117">updatedBy</span></span> | <span data-ttu-id="8bdfa-118">string</span><span class="sxs-lookup"><span data-stu-id="8bdfa-118">string</span></span> |<span data-ttu-id="8bdfa-119">テナント状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="8bdfa-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="8bdfa-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bdfa-120">updatedDateTime</span></span> | <span data-ttu-id="8bdfa-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bdfa-121">DateTimeOffset</span></span> |<span data-ttu-id="8bdfa-122">コントロールの状態が更新された時刻</span><span class="sxs-lookup"><span data-stu-id="8bdfa-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="8bdfa-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bdfa-123">JSON representation</span></span>
 <span data-ttu-id="8bdfa-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bdfa-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
