---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6849e333c6487029706c5a2485a174c10e665f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871849"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="cfb0a-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="cfb0a-103">installIntent enum type</span></span>

> <span data-ttu-id="cfb0a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfb0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfb0a-105">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="cfb0a-105">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="cfb0a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="cfb0a-106">Members</span></span>
|<span data-ttu-id="cfb0a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cfb0a-107">Member</span></span>|<span data-ttu-id="cfb0a-108">値</span><span class="sxs-lookup"><span data-stu-id="cfb0a-108">Value</span></span>|<span data-ttu-id="cfb0a-109">説明</span><span class="sxs-lookup"><span data-stu-id="cfb0a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfb0a-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="cfb0a-110">available</span></span>|<span data-ttu-id="cfb0a-111">0</span><span class="sxs-lookup"><span data-stu-id="cfb0a-111">0</span></span>|<span data-ttu-id="cfb0a-112">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="cfb0a-112">Available install intent.</span></span>|
|<span data-ttu-id="cfb0a-113">必須</span><span class="sxs-lookup"><span data-stu-id="cfb0a-113">required</span></span>|<span data-ttu-id="cfb0a-114">1</span><span class="sxs-lookup"><span data-stu-id="cfb0a-114">1</span></span>|<span data-ttu-id="cfb0a-115">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="cfb0a-115">Required install intent.</span></span>|
|<span data-ttu-id="cfb0a-116">アンインストール</span><span class="sxs-lookup"><span data-stu-id="cfb0a-116">uninstall</span></span>|<span data-ttu-id="cfb0a-117">2</span><span class="sxs-lookup"><span data-stu-id="cfb0a-117">2</span></span>|<span data-ttu-id="cfb0a-118">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="cfb0a-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="cfb0a-119">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="cfb0a-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="cfb0a-120">3</span><span class="sxs-lookup"><span data-stu-id="cfb0a-120">3</span></span>|<span data-ttu-id="cfb0a-121">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="cfb0a-121">Available without enrollment install intent.</span></span>|



