---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574391"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="e4540-103">secureScoreControlStateUpdate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4540-103">secureScoreControlStateUpdate resource type</span></span>

> <span data-ttu-id="e4540-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4540-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4540-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4540-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4540-106">ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。</span><span class="sxs-lookup"><span data-stu-id="e4540-106">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="e4540-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4540-107">Property</span></span>         | <span data-ttu-id="e4540-108">型</span><span class="sxs-lookup"><span data-stu-id="e4540-108">Type</span></span>           |<span data-ttu-id="e4540-109">説明</span><span class="sxs-lookup"><span data-stu-id="e4540-109">Description</span></span>                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| <span data-ttu-id="e4540-110">担当者</span><span class="sxs-lookup"><span data-stu-id="e4540-110">assignedTo</span></span>      | <span data-ttu-id="e4540-111">文字列</span><span class="sxs-lookup"><span data-stu-id="e4540-111">string</span></span>         | <span data-ttu-id="e4540-112">処理はユーザーにコントロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="e4540-112">Assign the control to the user who will take the action</span></span>     |
| <span data-ttu-id="e4540-113">comment</span><span class="sxs-lookup"><span data-stu-id="e4540-113">comment</span></span>         | <span data-ttu-id="e4540-114">文字列</span><span class="sxs-lookup"><span data-stu-id="e4540-114">string</span></span>         | <span data-ttu-id="e4540-115">コントロールに関するオプションのコメントを提供します。</span><span class="sxs-lookup"><span data-stu-id="e4540-115">Provides optional comment about the control</span></span>                 |
| <span data-ttu-id="e4540-116">state</span><span class="sxs-lookup"><span data-stu-id="e4540-116">state</span></span>           | <span data-ttu-id="e4540-117">文字列</span><span class="sxs-lookup"><span data-stu-id="e4540-117">string</span></span>         | <span data-ttu-id="e4540-118">修正プログラムのコマンドを使用してコントロールの状態を変更することができます (Ex: 無視され、サード ・ パーティなど)</span><span class="sxs-lookup"><span data-stu-id="e4540-118">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
| <span data-ttu-id="e4540-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="e4540-119">updatedBy</span></span>       | <span data-ttu-id="e4540-120">文字列</span><span class="sxs-lookup"><span data-stu-id="e4540-120">string</span></span>         |<span data-ttu-id="e4540-121">テナントの状態を更新したユーザーの ID</span><span class="sxs-lookup"><span data-stu-id="e4540-121">ID of the user who updated tenant state</span></span>                      |
| <span data-ttu-id="e4540-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4540-122">updatedDateTime</span></span> | <span data-ttu-id="e4540-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4540-123">DateTimeOffset</span></span> |<span data-ttu-id="e4540-124">コントロールの状態が更新された時間</span><span class="sxs-lookup"><span data-stu-id="e4540-124">Time at which control state was updated</span></span>                      |
 

## <a name="json-representation"></a><span data-ttu-id="e4540-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4540-125">JSON representation</span></span>
 <span data-ttu-id="e4540-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e4540-126">The following is a JSON representation of the resource.</span></span>

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
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
