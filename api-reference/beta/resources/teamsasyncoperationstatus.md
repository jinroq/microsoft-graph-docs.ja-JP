---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511710"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="3c7c4-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="3c7c4-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c7c4-104">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="3c7c4-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="3c7c4-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="3c7c4-105">Members</span></span>

| <span data-ttu-id="3c7c4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="3c7c4-106">Member</span></span> | <span data-ttu-id="3c7c4-107">値</span><span class="sxs-lookup"><span data-stu-id="3c7c4-107">Value</span></span>| <span data-ttu-id="3c7c4-108">説明</span><span class="sxs-lookup"><span data-stu-id="3c7c4-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3c7c4-109">Invalid</span><span class="sxs-lookup"><span data-stu-id="3c7c4-109">invalid</span></span>|<span data-ttu-id="3c7c4-110">(0)</span><span class="sxs-lookup"><span data-stu-id="3c7c4-110">0</span></span>|<span data-ttu-id="3c7c4-111">無効な値</span><span class="sxs-lookup"><span data-stu-id="3c7c4-111">Invalid value.</span></span>|
|<span data-ttu-id="3c7c4-112">NotStarted</span><span class="sxs-lookup"><span data-stu-id="3c7c4-112">notStarted</span></span>|<span data-ttu-id="3c7c4-113">-1</span><span class="sxs-lookup"><span data-stu-id="3c7c4-113">1</span></span>|<span data-ttu-id="3c7c4-114">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="3c7c4-114">The operation has not started.</span></span>|
|<span data-ttu-id="3c7c4-115">InProgress</span><span class="sxs-lookup"><span data-stu-id="3c7c4-115">inProgress</span></span>|<span data-ttu-id="3c7c4-116">-2</span><span class="sxs-lookup"><span data-stu-id="3c7c4-116">2</span></span>|<span data-ttu-id="3c7c4-117">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="3c7c4-117">The operation is running.</span></span>|
|<span data-ttu-id="3c7c4-118">Succeeded</span><span class="sxs-lookup"><span data-stu-id="3c7c4-118">succeeded</span></span>|<span data-ttu-id="3c7c4-119">-3</span><span class="sxs-lookup"><span data-stu-id="3c7c4-119">3</span></span>|<span data-ttu-id="3c7c4-120">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="3c7c4-120">The operation succeeded.</span></span>|
|<span data-ttu-id="3c7c4-121">Failed</span><span class="sxs-lookup"><span data-stu-id="3c7c4-121">failed</span></span>|<span data-ttu-id="3c7c4-122">-4</span><span class="sxs-lookup"><span data-stu-id="3c7c4-122">4</span></span>|<span data-ttu-id="3c7c4-123">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="3c7c4-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
