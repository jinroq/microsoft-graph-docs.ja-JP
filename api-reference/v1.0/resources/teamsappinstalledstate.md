---
title: メンバー
description: teamsapp の現在のインストール状態を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462250"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="f8e8e-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8e8e-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8e8e-104">[teamsapp](teamsapp.md)の現在のインストール状態を示します。</span><span class="sxs-lookup"><span data-stu-id="f8e8e-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="f8e8e-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8e8e-105">Members</span></span>

| <span data-ttu-id="f8e8e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8e8e-106">Member</span></span> | <span data-ttu-id="f8e8e-107">値</span><span class="sxs-lookup"><span data-stu-id="f8e8e-107">Value</span></span>| <span data-ttu-id="f8e8e-108">説明</span><span class="sxs-lookup"><span data-stu-id="f8e8e-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f8e8e-109">notinstalled</span><span class="sxs-lookup"><span data-stu-id="f8e8e-109">notInstalled</span></span>|<span data-ttu-id="f8e8e-110">.0</span><span class="sxs-lookup"><span data-stu-id="f8e8e-110">0</span></span>|<span data-ttu-id="f8e8e-111">アプリが team にインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="f8e8e-111">App is not installed to team.</span></span>|
|<span data-ttu-id="f8e8e-112">れる</span><span class="sxs-lookup"><span data-stu-id="f8e8e-112">installed</span></span>|<span data-ttu-id="f8e8e-113">1-d</span><span class="sxs-lookup"><span data-stu-id="f8e8e-113">1</span></span>|<span data-ttu-id="f8e8e-114">アプリは正常にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="f8e8e-114">App is installed normally.</span></span>|
|<span data-ttu-id="f8e8e-115">windows、および非推奨</span><span class="sxs-lookup"><span data-stu-id="f8e8e-115">installedAndHidden</span></span>|<span data-ttu-id="f8e8e-116">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f8e8e-116">2</span></span>|<span data-ttu-id="f8e8e-117">アプリはインストールされますが、ビューからは非表示になります。</span><span class="sxs-lookup"><span data-stu-id="f8e8e-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="f8e8e-118">windows viewer andパーマネント</span><span class="sxs-lookup"><span data-stu-id="f8e8e-118">installedAndPermanent</span></span>|<span data-ttu-id="f8e8e-119">1/3</span><span class="sxs-lookup"><span data-stu-id="f8e8e-119">3</span></span>|<span data-ttu-id="f8e8e-120">アプリは完全にインストールされており、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="f8e8e-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
