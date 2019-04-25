---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13436f259e254463874fe03217025380735e9b26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525237"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="54e40-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="54e40-103">installIntent enum type</span></span>

> <span data-ttu-id="54e40-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54e40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54e40-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54e40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54e40-106">管理者が選択したインストールの目的に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="54e40-106">Possible values for the install intent chosen by the admin.</span></span>

## <a name="members"></a><span data-ttu-id="54e40-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="54e40-107">Members</span></span>
|<span data-ttu-id="54e40-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="54e40-108">Member</span></span>|<span data-ttu-id="54e40-109">値</span><span class="sxs-lookup"><span data-stu-id="54e40-109">Value</span></span>|<span data-ttu-id="54e40-110">説明</span><span class="sxs-lookup"><span data-stu-id="54e40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54e40-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="54e40-111">available</span></span>|<span data-ttu-id="54e40-112">.0</span><span class="sxs-lookup"><span data-stu-id="54e40-112">0</span></span>|<span data-ttu-id="54e40-113">利用可能なインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="54e40-113">Available install intent.</span></span>|
|<span data-ttu-id="54e40-114">必須</span><span class="sxs-lookup"><span data-stu-id="54e40-114">required</span></span>|<span data-ttu-id="54e40-115">1 </span><span class="sxs-lookup"><span data-stu-id="54e40-115">1</span></span>|<span data-ttu-id="54e40-116">インストールの目的が必要です。</span><span class="sxs-lookup"><span data-stu-id="54e40-116">Required install intent.</span></span>|
|<span data-ttu-id="54e40-117">解除</span><span class="sxs-lookup"><span data-stu-id="54e40-117">uninstall</span></span>|<span data-ttu-id="54e40-118">2 </span><span class="sxs-lookup"><span data-stu-id="54e40-118">2</span></span>|<span data-ttu-id="54e40-119">インストールの目的をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="54e40-119">Uninstall install intent.</span></span>|
|<span data-ttu-id="54e40-120">登録なし</span><span class="sxs-lookup"><span data-stu-id="54e40-120">availableWithoutEnrollment</span></span>|<span data-ttu-id="54e40-121">3 </span><span class="sxs-lookup"><span data-stu-id="54e40-121">3</span></span>|<span data-ttu-id="54e40-122">登録インストールの目的がなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="54e40-122">Available without enrollment install intent.</span></span>|





