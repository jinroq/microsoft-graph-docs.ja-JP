---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、Default、ThirdParty、、レビュー済み) があります。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549140"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="b8b29-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8b29-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="b8b29-104">ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。</span><span class="sxs-lookup"><span data-stu-id="b8b29-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="b8b29-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8b29-105">Property</span></span> |<span data-ttu-id="b8b29-106">型</span><span class="sxs-lookup"><span data-stu-id="b8b29-106">Type</span></span> |<span data-ttu-id="b8b29-107">説明</span><span class="sxs-lookup"><span data-stu-id="b8b29-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="b8b29-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b8b29-108">assignedTo</span></span> | <span data-ttu-id="b8b29-109">string</span><span class="sxs-lookup"><span data-stu-id="b8b29-109">string</span></span> | <span data-ttu-id="b8b29-110">アクションを実行するユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b8b29-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="b8b29-111">comment</span><span class="sxs-lookup"><span data-stu-id="b8b29-111">comment</span></span> | <span data-ttu-id="b8b29-112">string</span><span class="sxs-lookup"><span data-stu-id="b8b29-112">string</span></span> | <span data-ttu-id="b8b29-113">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="b8b29-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="b8b29-114">state</span><span class="sxs-lookup"><span data-stu-id="b8b29-114">state</span></span> | <span data-ttu-id="b8b29-115">string</span><span class="sxs-lookup"><span data-stu-id="b8b29-115">string</span></span> | <span data-ttu-id="b8b29-116">PATCH コマンドを使用してコントロールの状態を変更できます (例: 無視、thirdParty など)</span><span class="sxs-lookup"><span data-stu-id="b8b29-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="b8b29-117">updatedby</span><span class="sxs-lookup"><span data-stu-id="b8b29-117">updatedBy</span></span> | <span data-ttu-id="b8b29-118">string</span><span class="sxs-lookup"><span data-stu-id="b8b29-118">string</span></span> |<span data-ttu-id="b8b29-119">テナント状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="b8b29-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="b8b29-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b29-120">updatedDateTime</span></span> | <span data-ttu-id="b8b29-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="b8b29-121">DateTimeOffset?</span></span> |<span data-ttu-id="b8b29-122">コントロールの状態が更新された時刻</span><span class="sxs-lookup"><span data-stu-id="b8b29-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="b8b29-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8b29-123">JSON representation</span></span>
 <span data-ttu-id="b8b29-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8b29-124">The following is a JSON representation of the resource.</span></span>
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
