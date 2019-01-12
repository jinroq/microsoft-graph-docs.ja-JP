---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aaea49b0c808b0591a059f46ed0eb06fa17b6177
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972055"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="5a864-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="5a864-103">installIntent enum type</span></span>

> <span data-ttu-id="5a864-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a864-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a864-105">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="5a864-105">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="5a864-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a864-106">Members</span></span>
|<span data-ttu-id="5a864-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a864-107">Member</span></span>|<span data-ttu-id="5a864-108">値</span><span class="sxs-lookup"><span data-stu-id="5a864-108">Value</span></span>|<span data-ttu-id="5a864-109">説明</span><span class="sxs-lookup"><span data-stu-id="5a864-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a864-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="5a864-110">available</span></span>|<span data-ttu-id="5a864-111">0</span><span class="sxs-lookup"><span data-stu-id="5a864-111">0</span></span>|<span data-ttu-id="5a864-112">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="5a864-112">Available install intent.</span></span>|
|<span data-ttu-id="5a864-113">必須</span><span class="sxs-lookup"><span data-stu-id="5a864-113">required</span></span>|<span data-ttu-id="5a864-114">1</span><span class="sxs-lookup"><span data-stu-id="5a864-114">1</span></span>|<span data-ttu-id="5a864-115">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="5a864-115">Required install intent.</span></span>|
|<span data-ttu-id="5a864-116">アンインストール</span><span class="sxs-lookup"><span data-stu-id="5a864-116">uninstall</span></span>|<span data-ttu-id="5a864-117">2</span><span class="sxs-lookup"><span data-stu-id="5a864-117">2</span></span>|<span data-ttu-id="5a864-118">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="5a864-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="5a864-119">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="5a864-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="5a864-120">3</span><span class="sxs-lookup"><span data-stu-id="5a864-120">3</span></span>|<span data-ttu-id="5a864-121">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="5a864-121">Available without enrollment install intent.</span></span>|



