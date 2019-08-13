---
title: windowsPrivacyDataAccessLevel 列挙型
description: 特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 507252538606ccb47d72e8dc60710de04acc9b09
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369648"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="24aec-103">windowsPrivacyDataAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="24aec-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="24aec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24aec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24aec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24aec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24aec-106">特定の Windows プライバシーデータカテゴリへのアクセスレベルを決定します。</span><span class="sxs-lookup"><span data-stu-id="24aec-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="24aec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="24aec-107">Members</span></span>
|<span data-ttu-id="24aec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="24aec-108">Member</span></span>|<span data-ttu-id="24aec-109">値</span><span class="sxs-lookup"><span data-stu-id="24aec-109">Value</span></span>|<span data-ttu-id="24aec-110">説明</span><span class="sxs-lookup"><span data-stu-id="24aec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24aec-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="24aec-111">notConfigured</span></span>|<span data-ttu-id="24aec-112">.0</span><span class="sxs-lookup"><span data-stu-id="24aec-112">0</span></span>|<span data-ttu-id="24aec-113">指定されたアクセスレベルはありません。意図的なものではありません。</span><span class="sxs-lookup"><span data-stu-id="24aec-113">No access level specified, no intents.</span></span> <span data-ttu-id="24aec-114">デバイスは UserInControl または ForceAllow のどちらかの動作をすることがあります。</span><span class="sxs-lookup"><span data-stu-id="24aec-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="24aec-115">アクセスされたプライバシーデータ、Windows のバージョン、その他の要因によって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="24aec-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="24aec-116">forceAllow</span><span class="sxs-lookup"><span data-stu-id="24aec-116">forceAllow</span></span>|<span data-ttu-id="24aec-117">1-d</span><span class="sxs-lookup"><span data-stu-id="24aec-117">1</span></span>|<span data-ttu-id="24aec-118">アプリは、指定されたプライバシーデータにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="24aec-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="24aec-119">forceDeny</span><span class="sxs-lookup"><span data-stu-id="24aec-119">forceDeny</span></span>|<span data-ttu-id="24aec-120">pbm-2</span><span class="sxs-lookup"><span data-stu-id="24aec-120">2</span></span>|<span data-ttu-id="24aec-121">アプリは、指定されたプライバシーデータにアクセスすることを拒否されます。</span><span class="sxs-lookup"><span data-stu-id="24aec-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="24aec-122">userInControl</span><span class="sxs-lookup"><span data-stu-id="24aec-122">userInControl</span></span>|<span data-ttu-id="24aec-123">1/3</span><span class="sxs-lookup"><span data-stu-id="24aec-123">3</span></span>|<span data-ttu-id="24aec-124">アプリが指定されたプライバシーデータにアクセスしようとすると、ユーザーにメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="24aec-124">Users will be prompted when apps try to access specified privacy data.</span></span>|



