---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a6c000524d8179643b4a32d47ca05df9c7b32de
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161258"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="f3f56-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="f3f56-103">installIntent enum type</span></span>

> <span data-ttu-id="f3f56-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3f56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3f56-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3f56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f56-106">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="f3f56-106">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="f3f56-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3f56-107">Members</span></span>
|<span data-ttu-id="f3f56-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3f56-108">Member</span></span>|<span data-ttu-id="f3f56-109">値</span><span class="sxs-lookup"><span data-stu-id="f3f56-109">Value</span></span>|<span data-ttu-id="f3f56-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3f56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f56-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="f3f56-111">available</span></span>|<span data-ttu-id="f3f56-112">.0</span><span class="sxs-lookup"><span data-stu-id="f3f56-112">0</span></span>|<span data-ttu-id="f3f56-113">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="f3f56-113">Available install intent.</span></span>|
|<span data-ttu-id="f3f56-114">必須</span><span class="sxs-lookup"><span data-stu-id="f3f56-114">required</span></span>|<span data-ttu-id="f3f56-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f3f56-115">1</span></span>|<span data-ttu-id="f3f56-116">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3f56-116">Required install intent.</span></span>|
|<span data-ttu-id="f3f56-117">解除</span><span class="sxs-lookup"><span data-stu-id="f3f56-117">uninstall</span></span>|<span data-ttu-id="f3f56-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f3f56-118">2</span></span>|<span data-ttu-id="f3f56-119">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="f3f56-119">Uninstall install intent.</span></span>|
|<span data-ttu-id="f3f56-120">登録なし</span><span class="sxs-lookup"><span data-stu-id="f3f56-120">availableWithoutEnrollment</span></span>|<span data-ttu-id="f3f56-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f3f56-121">3</span></span>|<span data-ttu-id="f3f56-122">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="f3f56-122">Available without enrollment install intent.</span></span>|




