---
title: mobileAppDependencyType 列挙型
description: 2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ca22fd9b62e0affbf3a3a945c417e8695267a81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957067"
---
# <a name="mobileappdependencytype-enum-type"></a><span data-ttu-id="07251-103">mobileAppDependencyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="07251-103">mobileAppDependencyType enum type</span></span>

> <span data-ttu-id="07251-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07251-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07251-106">2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="07251-106">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="07251-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="07251-107">Members</span></span>
|<span data-ttu-id="07251-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="07251-108">Member</span></span>|<span data-ttu-id="07251-109">値</span><span class="sxs-lookup"><span data-stu-id="07251-109">Value</span></span>|<span data-ttu-id="07251-110">説明</span><span class="sxs-lookup"><span data-stu-id="07251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07251-111">検出</span><span class="sxs-lookup"><span data-stu-id="07251-111">detect</span></span>|<span data-ttu-id="07251-112">.0</span><span class="sxs-lookup"><span data-stu-id="07251-112">0</span></span>|<span data-ttu-id="07251-113">親アプリをインストールする前に、子アプリを検出する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="07251-113">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="07251-114">自動</span><span class="sxs-lookup"><span data-stu-id="07251-114">autoInstall</span></span>|<span data-ttu-id="07251-115">1-d</span><span class="sxs-lookup"><span data-stu-id="07251-115">1</span></span>|<span data-ttu-id="07251-116">親アプリをインストールする前に、子アプリをインストールする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="07251-116">Indicates that the child app should be installed before installing the parent app.</span></span>|




