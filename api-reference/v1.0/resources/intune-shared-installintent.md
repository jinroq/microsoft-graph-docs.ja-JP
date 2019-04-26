---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40c36022e08917ac8fbad0ff2647e28da18270bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571906"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="d5400-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5400-103">installIntent enum type</span></span>

> <span data-ttu-id="d5400-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5400-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5400-105">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="d5400-105">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="d5400-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5400-106">Members</span></span>
|<span data-ttu-id="d5400-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5400-107">Member</span></span>|<span data-ttu-id="d5400-108">値</span><span class="sxs-lookup"><span data-stu-id="d5400-108">Value</span></span>|<span data-ttu-id="d5400-109">説明</span><span class="sxs-lookup"><span data-stu-id="d5400-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5400-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="d5400-110">available</span></span>|<span data-ttu-id="d5400-111">.0</span><span class="sxs-lookup"><span data-stu-id="d5400-111">0</span></span>|<span data-ttu-id="d5400-112">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="d5400-112">Available install intent.</span></span>|
|<span data-ttu-id="d5400-113">必須</span><span class="sxs-lookup"><span data-stu-id="d5400-113">required</span></span>|<span data-ttu-id="d5400-114">1 </span><span class="sxs-lookup"><span data-stu-id="d5400-114">1</span></span>|<span data-ttu-id="d5400-115">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5400-115">Required install intent.</span></span>|
|<span data-ttu-id="d5400-116">解除</span><span class="sxs-lookup"><span data-stu-id="d5400-116">uninstall</span></span>|<span data-ttu-id="d5400-117">2 </span><span class="sxs-lookup"><span data-stu-id="d5400-117">2</span></span>|<span data-ttu-id="d5400-118">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="d5400-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="d5400-119">登録なし</span><span class="sxs-lookup"><span data-stu-id="d5400-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="d5400-120">3 </span><span class="sxs-lookup"><span data-stu-id="d5400-120">3</span></span>|<span data-ttu-id="d5400-121">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="d5400-121">Available without enrollment install intent.</span></span>|



