---
title: mobileAppDependecyType 列挙型
description: 2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cbf468435aa289913b566750823e65c73249838
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808976"
---
# <a name="mobileappdependecytype-enum-type"></a><span data-ttu-id="d6876-103">mobileAppDependecyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6876-103">mobileAppDependecyType enum type</span></span>

> <span data-ttu-id="d6876-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6876-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6876-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6876-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6876-106">2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d6876-106">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="d6876-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6876-107">Members</span></span>
|<span data-ttu-id="d6876-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6876-108">Member</span></span>|<span data-ttu-id="d6876-109">値</span><span class="sxs-lookup"><span data-stu-id="d6876-109">Value</span></span>|<span data-ttu-id="d6876-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6876-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6876-111">検出</span><span class="sxs-lookup"><span data-stu-id="d6876-111">detect</span></span>|<span data-ttu-id="d6876-112">.0</span><span class="sxs-lookup"><span data-stu-id="d6876-112">0</span></span>|<span data-ttu-id="d6876-113">親アプリをインストールする前に、子アプリを検出する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d6876-113">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="d6876-114">自動</span><span class="sxs-lookup"><span data-stu-id="d6876-114">autoInstall</span></span>|<span data-ttu-id="d6876-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d6876-115">1</span></span>|<span data-ttu-id="d6876-116">親アプリをインストールする前に、子アプリをインストールする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d6876-116">Indicates that the child app should be installed before installing the parent app.</span></span>|





