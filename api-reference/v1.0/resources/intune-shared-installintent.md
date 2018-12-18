---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
author: tfitzmac
ms.openlocfilehash: 6b14dae67f8590e3b38865b80a385babf032f16a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303662"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="e56ea-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="e56ea-103">installIntent enum type</span></span>

> <span data-ttu-id="e56ea-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e56ea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e56ea-105">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="e56ea-105">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="e56ea-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e56ea-106">Members</span></span>
|<span data-ttu-id="e56ea-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e56ea-107">Member</span></span>|<span data-ttu-id="e56ea-108">値</span><span class="sxs-lookup"><span data-stu-id="e56ea-108">Value</span></span>|<span data-ttu-id="e56ea-109">説明</span><span class="sxs-lookup"><span data-stu-id="e56ea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e56ea-110">使用可能</span><span class="sxs-lookup"><span data-stu-id="e56ea-110">available</span></span>|<span data-ttu-id="e56ea-111">0</span><span class="sxs-lookup"><span data-stu-id="e56ea-111">0</span></span>|<span data-ttu-id="e56ea-112">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="e56ea-112">Available install intent.</span></span>|
|<span data-ttu-id="e56ea-113">必須</span><span class="sxs-lookup"><span data-stu-id="e56ea-113">required</span></span>|<span data-ttu-id="e56ea-114">1</span><span class="sxs-lookup"><span data-stu-id="e56ea-114">1</span></span>|<span data-ttu-id="e56ea-115">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="e56ea-115">Required install intent.</span></span>|
|<span data-ttu-id="e56ea-116">アンインストール</span><span class="sxs-lookup"><span data-stu-id="e56ea-116">uninstall</span></span>|<span data-ttu-id="e56ea-117">2</span><span class="sxs-lookup"><span data-stu-id="e56ea-117">2</span></span>|<span data-ttu-id="e56ea-118">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="e56ea-118">Uninstall install intent.</span></span>|
|<span data-ttu-id="e56ea-119">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="e56ea-119">availableWithoutEnrollment</span></span>|<span data-ttu-id="e56ea-120">3</span><span class="sxs-lookup"><span data-stu-id="e56ea-120">3</span></span>|<span data-ttu-id="e56ea-121">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="e56ea-121">Available without enrollment install intent.</span></span>|



