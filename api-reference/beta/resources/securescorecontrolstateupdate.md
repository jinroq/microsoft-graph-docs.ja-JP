---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/22/2018
ms.locfileid: "27428841"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="f7329-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7329-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="f7329-104">ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。</span><span class="sxs-lookup"><span data-stu-id="f7329-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="f7329-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7329-105">Property</span></span> |<span data-ttu-id="f7329-106">型</span><span class="sxs-lookup"><span data-stu-id="f7329-106">Type</span></span> |<span data-ttu-id="f7329-107">説明</span><span class="sxs-lookup"><span data-stu-id="f7329-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="f7329-108">担当者</span><span class="sxs-lookup"><span data-stu-id="f7329-108">assignedTo</span></span> | <span data-ttu-id="f7329-109">文字列</span><span class="sxs-lookup"><span data-stu-id="f7329-109">string</span></span> | <span data-ttu-id="f7329-110">処理はユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="f7329-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="f7329-111">comment</span><span class="sxs-lookup"><span data-stu-id="f7329-111">comment</span></span> | <span data-ttu-id="f7329-112">文字列</span><span class="sxs-lookup"><span data-stu-id="f7329-112">string</span></span> | <span data-ttu-id="f7329-113">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="f7329-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="f7329-114">state</span><span class="sxs-lookup"><span data-stu-id="f7329-114">state</span></span> | <span data-ttu-id="f7329-115">文字列</span><span class="sxs-lookup"><span data-stu-id="f7329-115">string</span></span> | <span data-ttu-id="f7329-116">修正プログラムのコマンドを使用してコントロールの状態を変更することができます (Ex: 無視され、サード ・ パーティなど)</span><span class="sxs-lookup"><span data-stu-id="f7329-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="f7329-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="f7329-117">updatedBy</span></span> | <span data-ttu-id="f7329-118">文字列</span><span class="sxs-lookup"><span data-stu-id="f7329-118">string</span></span> |<span data-ttu-id="f7329-119">テナントの状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="f7329-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="f7329-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7329-120">updatedDateTime</span></span> | <span data-ttu-id="f7329-121">DateTimeOffset でしょうか。</span><span class="sxs-lookup"><span data-stu-id="f7329-121">DateTimeOffset?</span></span> |<span data-ttu-id="f7329-122">コントロールの状態が更新された時間</span><span class="sxs-lookup"><span data-stu-id="f7329-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="f7329-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7329-123">JSON representation</span></span>
 <span data-ttu-id="f7329-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7329-124">The following is a JSON representation of the resource.</span></span>
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
