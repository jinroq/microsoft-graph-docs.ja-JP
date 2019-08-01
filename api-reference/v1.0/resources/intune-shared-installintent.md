---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab42bde2c31537371ae1fd7e3b248bbdfce964ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036898"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="ec80a-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec80a-103">installIntent enum type</span></span>

> <span data-ttu-id="ec80a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec80a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec80a-105">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="ec80a-105">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="ec80a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec80a-106">Members</span></span>
|<span data-ttu-id="ec80a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec80a-107">Member</span></span>|<span data-ttu-id="ec80a-108">値</span><span class="sxs-lookup"><span data-stu-id="ec80a-108">Value</span></span>|<span data-ttu-id="ec80a-109">説明</span><span class="sxs-lookup"><span data-stu-id="ec80a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec80a-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="ec80a-110">available</span></span>|<span data-ttu-id="ec80a-111">.0</span><span class="sxs-lookup"><span data-stu-id="ec80a-111">0</span></span>|<span data-ttu-id="ec80a-112">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="ec80a-112">Available install intent.</span></span>|
|<span data-ttu-id="ec80a-113">必須</span><span class="sxs-lookup"><span data-stu-id="ec80a-113">required</span></span>|<span data-ttu-id="ec80a-114">1-d</span><span class="sxs-lookup"><span data-stu-id="ec80a-114">1</span></span>|<span data-ttu-id="ec80a-115">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec80a-115">Required install intent.</span></span>|
|<span data-ttu-id="ec80a-116">解除</span><span class="sxs-lookup"><span data-stu-id="ec80a-116">uninstall</span></span>|<span data-ttu-id="ec80a-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ec80a-117">2</span></span>|<span data-ttu-id="ec80a-118">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="ec80a-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="ec80a-119">登録なし</span><span class="sxs-lookup"><span data-stu-id="ec80a-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="ec80a-120">1/3</span><span class="sxs-lookup"><span data-stu-id="ec80a-120">3</span></span>|<span data-ttu-id="ec80a-121">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="ec80a-121">Available without enrollment install intent.</span></span>|



