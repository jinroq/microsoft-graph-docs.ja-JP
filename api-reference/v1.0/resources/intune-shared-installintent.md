---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40c36022e08917ac8fbad0ff2647e28da18270bc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260418"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="27523-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="27523-103">installIntent enum type</span></span>

> <span data-ttu-id="27523-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27523-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27523-105">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="27523-105">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="27523-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="27523-106">Members</span></span>
|<span data-ttu-id="27523-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="27523-107">Member</span></span>|<span data-ttu-id="27523-108">値</span><span class="sxs-lookup"><span data-stu-id="27523-108">Value</span></span>|<span data-ttu-id="27523-109">説明</span><span class="sxs-lookup"><span data-stu-id="27523-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27523-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="27523-110">available</span></span>|<span data-ttu-id="27523-111">.0</span><span class="sxs-lookup"><span data-stu-id="27523-111">0</span></span>|<span data-ttu-id="27523-112">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="27523-112">Available install intent.</span></span>|
|<span data-ttu-id="27523-113">必須</span><span class="sxs-lookup"><span data-stu-id="27523-113">required</span></span>|<span data-ttu-id="27523-114">1-d</span><span class="sxs-lookup"><span data-stu-id="27523-114">1</span></span>|<span data-ttu-id="27523-115">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="27523-115">Required install intent.</span></span>|
|<span data-ttu-id="27523-116">解除</span><span class="sxs-lookup"><span data-stu-id="27523-116">uninstall</span></span>|<span data-ttu-id="27523-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="27523-117">2</span></span>|<span data-ttu-id="27523-118">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="27523-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="27523-119">登録なし</span><span class="sxs-lookup"><span data-stu-id="27523-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="27523-120">1/3</span><span class="sxs-lookup"><span data-stu-id="27523-120">3</span></span>|<span data-ttu-id="27523-121">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="27523-121">Available without enrollment install intent.</span></span>|



