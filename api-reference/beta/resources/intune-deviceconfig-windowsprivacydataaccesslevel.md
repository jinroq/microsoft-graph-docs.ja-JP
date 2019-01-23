---
title: windowsPrivacyDataAccessLevel 列挙型
description: Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410624"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="88884-103">windowsPrivacyDataAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="88884-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="88884-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="88884-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88884-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88884-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88884-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88884-107">Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。</span><span class="sxs-lookup"><span data-stu-id="88884-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="88884-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="88884-108">Members</span></span>
|<span data-ttu-id="88884-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="88884-109">Member</span></span>|<span data-ttu-id="88884-110">値</span><span class="sxs-lookup"><span data-stu-id="88884-110">Value</span></span>|<span data-ttu-id="88884-111">説明</span><span class="sxs-lookup"><span data-stu-id="88884-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88884-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="88884-112">notConfigured</span></span>|<span data-ttu-id="88884-113">0</span><span class="sxs-lookup"><span data-stu-id="88884-113">0</span></span>|<span data-ttu-id="88884-114">目的なしアクセス レベルが指定されませんでした。</span><span class="sxs-lookup"><span data-stu-id="88884-114">No access level specified, no intents.</span></span> <span data-ttu-id="88884-115">デバイスは、UserInControl や ForceAllow のように動作可能性があります。</span><span class="sxs-lookup"><span data-stu-id="88884-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="88884-116">プライバシー ・ データによりますが、されたバージョンの Windows およびその他の要素にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="88884-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="88884-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="88884-117">forceAllow</span></span>|<span data-ttu-id="88884-118">1</span><span class="sxs-lookup"><span data-stu-id="88884-118">1</span></span>|<span data-ttu-id="88884-119">アプリケーションは、指定したプライバシー データへのアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="88884-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="88884-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="88884-120">forceDeny</span></span>|<span data-ttu-id="88884-121">2</span><span class="sxs-lookup"><span data-stu-id="88884-121">2</span></span>|<span data-ttu-id="88884-122">指定したプライバシー ・ データにアクセスするアプリケーションは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="88884-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="88884-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="88884-123">userInControl</span></span>|<span data-ttu-id="88884-124">3</span><span class="sxs-lookup"><span data-stu-id="88884-124">3</span></span>|<span data-ttu-id="88884-125">アプリケーションが指定したプライバシー ・ データにアクセスしようとした場合、ユーザーが要求されます。</span><span class="sxs-lookup"><span data-stu-id="88884-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




