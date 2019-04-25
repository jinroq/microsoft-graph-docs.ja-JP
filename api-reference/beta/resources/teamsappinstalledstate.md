---
title: Members
description: teamsapp の現在のインストール状態を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554017"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="a9ced-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="a9ced-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ced-104">[teamsapp](teamsapp.md)の現在のインストール状態を示します。</span><span class="sxs-lookup"><span data-stu-id="a9ced-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="a9ced-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="a9ced-105">Members</span></span>

| <span data-ttu-id="a9ced-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a9ced-106">Member</span></span> | <span data-ttu-id="a9ced-107">値</span><span class="sxs-lookup"><span data-stu-id="a9ced-107">Value</span></span>| <span data-ttu-id="a9ced-108">説明</span><span class="sxs-lookup"><span data-stu-id="a9ced-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a9ced-109">notinstalled</span><span class="sxs-lookup"><span data-stu-id="a9ced-109">notInstalled</span></span>|<span data-ttu-id="a9ced-110">.0</span><span class="sxs-lookup"><span data-stu-id="a9ced-110">0</span></span>|<span data-ttu-id="a9ced-111">アプリが team にインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ced-111">App is not installed to team.</span></span>|
|<span data-ttu-id="a9ced-112">れる</span><span class="sxs-lookup"><span data-stu-id="a9ced-112">installed</span></span>|<span data-ttu-id="a9ced-113">1 </span><span class="sxs-lookup"><span data-stu-id="a9ced-113">1</span></span>|<span data-ttu-id="a9ced-114">アプリは正常にインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a9ced-114">App is installed normally.</span></span>|
|<span data-ttu-id="a9ced-115">windows、および非推奨</span><span class="sxs-lookup"><span data-stu-id="a9ced-115">installedAndHidden</span></span>|<span data-ttu-id="a9ced-116">2 </span><span class="sxs-lookup"><span data-stu-id="a9ced-116">2</span></span>|<span data-ttu-id="a9ced-117">アプリはインストールされますが、ビューからは非表示になります。</span><span class="sxs-lookup"><span data-stu-id="a9ced-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="a9ced-118">windows viewer andパーマネント</span><span class="sxs-lookup"><span data-stu-id="a9ced-118">installedAndPermanent</span></span>|<span data-ttu-id="a9ced-119">3 </span><span class="sxs-lookup"><span data-stu-id="a9ced-119">3</span></span>|<span data-ttu-id="a9ced-120">アプリは完全にインストールされており、削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="a9ced-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
