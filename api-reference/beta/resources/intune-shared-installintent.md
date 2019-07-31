---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 77b2dcadade32a817f0cb482e32871660ad3b06f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010449"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="3287e-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="3287e-103">installIntent enum type</span></span>

> <span data-ttu-id="3287e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3287e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3287e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3287e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3287e-106">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="3287e-106">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="3287e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3287e-107">Members</span></span>
|<span data-ttu-id="3287e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3287e-108">Member</span></span>|<span data-ttu-id="3287e-109">値</span><span class="sxs-lookup"><span data-stu-id="3287e-109">Value</span></span>|<span data-ttu-id="3287e-110">説明</span><span class="sxs-lookup"><span data-stu-id="3287e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3287e-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="3287e-111">available</span></span>|<span data-ttu-id="3287e-112">.0</span><span class="sxs-lookup"><span data-stu-id="3287e-112">0</span></span>|<span data-ttu-id="3287e-113">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="3287e-113">Available install intent.</span></span>|
|<span data-ttu-id="3287e-114">必須</span><span class="sxs-lookup"><span data-stu-id="3287e-114">required</span></span>|<span data-ttu-id="3287e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3287e-115">1</span></span>|<span data-ttu-id="3287e-116">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="3287e-116">Required install intent.</span></span>|
|<span data-ttu-id="3287e-117">解除</span><span class="sxs-lookup"><span data-stu-id="3287e-117">uninstall</span></span>|<span data-ttu-id="3287e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3287e-118">2</span></span>|<span data-ttu-id="3287e-119">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="3287e-119">Uninstall install intent.</span></span>|
|<span data-ttu-id="3287e-120">登録なし</span><span class="sxs-lookup"><span data-stu-id="3287e-120">availableWithoutEnrollment</span></span>|<span data-ttu-id="3287e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3287e-121">3</span></span>|<span data-ttu-id="3287e-122">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="3287e-122">Available without enrollment install intent.</span></span>|





