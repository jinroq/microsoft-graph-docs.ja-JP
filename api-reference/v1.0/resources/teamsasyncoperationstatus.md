---
title: teamsAsyncOperationStatus 列挙型
description: teamsAsyncOperation の現在の状態を表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3ceaca73fe013b76f44cdf9290f3c0935e93b0a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462229"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="f7bbf-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7bbf-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7bbf-104">[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="f7bbf-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7bbf-105">Members</span></span>

| <span data-ttu-id="f7bbf-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7bbf-106">Member</span></span> | <span data-ttu-id="f7bbf-107">値</span><span class="sxs-lookup"><span data-stu-id="f7bbf-107">Value</span></span>| <span data-ttu-id="f7bbf-108">説明</span><span class="sxs-lookup"><span data-stu-id="f7bbf-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f7bbf-109">無効です</span><span class="sxs-lookup"><span data-stu-id="f7bbf-109">invalid</span></span>|<span data-ttu-id="f7bbf-110">.0</span><span class="sxs-lookup"><span data-stu-id="f7bbf-110">0</span></span>|<span data-ttu-id="f7bbf-111">無効な値です。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-111">Invalid value.</span></span>|
|<span data-ttu-id="f7bbf-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="f7bbf-112">notStarted</span></span>|<span data-ttu-id="f7bbf-113">1-d</span><span class="sxs-lookup"><span data-stu-id="f7bbf-113">1</span></span>|<span data-ttu-id="f7bbf-114">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-114">The operation has not started.</span></span>|
|<span data-ttu-id="f7bbf-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="f7bbf-115">inProgress</span></span>|<span data-ttu-id="f7bbf-116">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f7bbf-116">2</span></span>|<span data-ttu-id="f7bbf-117">操作が実行されています。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-117">The operation is running.</span></span>|
|<span data-ttu-id="f7bbf-118">失敗</span><span class="sxs-lookup"><span data-stu-id="f7bbf-118">succeeded</span></span>|<span data-ttu-id="f7bbf-119">1/3</span><span class="sxs-lookup"><span data-stu-id="f7bbf-119">3</span></span>|<span data-ttu-id="f7bbf-120">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-120">The operation succeeded.</span></span>|
|<span data-ttu-id="f7bbf-121">フェール</span><span class="sxs-lookup"><span data-stu-id="f7bbf-121">failed</span></span>|<span data-ttu-id="f7bbf-122">2/4</span><span class="sxs-lookup"><span data-stu-id="f7bbf-122">4</span></span>|<span data-ttu-id="f7bbf-123">操作は失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f7bbf-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
