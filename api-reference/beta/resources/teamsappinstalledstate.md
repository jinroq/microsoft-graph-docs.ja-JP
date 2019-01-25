---
title: Members
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517275"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="c7fb6-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="c7fb6-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7fb6-104">の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="c7fb6-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7fb6-105">Members</span></span>

| <span data-ttu-id="c7fb6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7fb6-106">Member</span></span> | <span data-ttu-id="c7fb6-107">値</span><span class="sxs-lookup"><span data-stu-id="c7fb6-107">Value</span></span>| <span data-ttu-id="c7fb6-108">説明</span><span class="sxs-lookup"><span data-stu-id="c7fb6-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c7fb6-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="c7fb6-109">notInstalled</span></span>|<span data-ttu-id="c7fb6-110">(0)</span><span class="sxs-lookup"><span data-stu-id="c7fb6-110">0</span></span>|<span data-ttu-id="c7fb6-111">チームには、アプリケーションはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-111">App is not installed to team.</span></span>|
|<span data-ttu-id="c7fb6-112">Installed</span><span class="sxs-lookup"><span data-stu-id="c7fb6-112">installed</span></span>|<span data-ttu-id="c7fb6-113">-1</span><span class="sxs-lookup"><span data-stu-id="c7fb6-113">1</span></span>|<span data-ttu-id="c7fb6-114">アプリケーションが正常にインストールします。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-114">App is installed normally.</span></span>|
|<span data-ttu-id="c7fb6-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="c7fb6-115">installedAndHidden</span></span>|<span data-ttu-id="c7fb6-116">-2</span><span class="sxs-lookup"><span data-stu-id="c7fb6-116">2</span></span>|<span data-ttu-id="c7fb6-117">アプリケーションがインストールされているがビューから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="c7fb6-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="c7fb6-118">installedAndPermanent</span></span>|<span data-ttu-id="c7fb6-119">-3</span><span class="sxs-lookup"><span data-stu-id="c7fb6-119">3</span></span>|<span data-ttu-id="c7fb6-120">アプリケーションが完全にインストールされているしは削除できません。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
