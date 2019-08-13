---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3f8307445360a1b0dd43c8a164dd1f2d8032562
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348022"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="fa134-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="fa134-103">installIntent enum type</span></span>

> <span data-ttu-id="fa134-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa134-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa134-106">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="fa134-106">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="fa134-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fa134-107">Members</span></span>
|<span data-ttu-id="fa134-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fa134-108">Member</span></span>|<span data-ttu-id="fa134-109">値</span><span class="sxs-lookup"><span data-stu-id="fa134-109">Value</span></span>|<span data-ttu-id="fa134-110">説明</span><span class="sxs-lookup"><span data-stu-id="fa134-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa134-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="fa134-111">available</span></span>|<span data-ttu-id="fa134-112">.0</span><span class="sxs-lookup"><span data-stu-id="fa134-112">0</span></span>|<span data-ttu-id="fa134-113">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="fa134-113">Available install intent.</span></span>|
|<span data-ttu-id="fa134-114">必須</span><span class="sxs-lookup"><span data-stu-id="fa134-114">required</span></span>|<span data-ttu-id="fa134-115">1-d</span><span class="sxs-lookup"><span data-stu-id="fa134-115">1</span></span>|<span data-ttu-id="fa134-116">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa134-116">Required install intent.</span></span>|
|<span data-ttu-id="fa134-117">解除</span><span class="sxs-lookup"><span data-stu-id="fa134-117">uninstall</span></span>|<span data-ttu-id="fa134-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="fa134-118">2</span></span>|<span data-ttu-id="fa134-119">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="fa134-119">Uninstall install intent.</span></span>|
|<span data-ttu-id="fa134-120">登録なし</span><span class="sxs-lookup"><span data-stu-id="fa134-120">availableWithoutEnrollment</span></span>|<span data-ttu-id="fa134-121">1/3</span><span class="sxs-lookup"><span data-stu-id="fa134-121">3</span></span>|<span data-ttu-id="fa134-122">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="fa134-122">Available without enrollment install intent.</span></span>|



