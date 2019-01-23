---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 812aacf65bc73aade6eafc441fafda914ea6a3b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423301"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="da433-103">subjectAlternativeNameType 列挙型</span><span class="sxs-lookup"><span data-stu-id="da433-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="da433-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da433-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da433-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da433-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da433-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da433-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da433-107">サブジェクト代替名のオプションです。</span><span class="sxs-lookup"><span data-stu-id="da433-107">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="da433-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="da433-108">Members</span></span>
|<span data-ttu-id="da433-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="da433-109">Member</span></span>|<span data-ttu-id="da433-110">値</span><span class="sxs-lookup"><span data-stu-id="da433-110">Value</span></span>|<span data-ttu-id="da433-111">説明</span><span class="sxs-lookup"><span data-stu-id="da433-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da433-112">none</span><span class="sxs-lookup"><span data-stu-id="da433-112">none</span></span>|<span data-ttu-id="da433-113">0</span><span class="sxs-lookup"><span data-stu-id="da433-113">0</span></span>|<span data-ttu-id="da433-114">サブジェクト代替名がありません。</span><span class="sxs-lookup"><span data-stu-id="da433-114">No subject alternative name.</span></span>|
|<span data-ttu-id="da433-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="da433-115">emailAddress</span></span>|<span data-ttu-id="da433-116">1</span><span class="sxs-lookup"><span data-stu-id="da433-116">1</span></span>|<span data-ttu-id="da433-117">電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="da433-117">Email address.</span></span>|
|<span data-ttu-id="da433-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="da433-118">userPrincipalName</span></span>|<span data-ttu-id="da433-119">2</span><span class="sxs-lookup"><span data-stu-id="da433-119">2</span></span>|<span data-ttu-id="da433-120">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="da433-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="da433-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="da433-121">customAzureADAttribute</span></span>|<span data-ttu-id="da433-122">4</span><span class="sxs-lookup"><span data-stu-id="da433-122">4</span></span>|<span data-ttu-id="da433-123">Azure の AD 属性をカスタムします。</span><span class="sxs-lookup"><span data-stu-id="da433-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="da433-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="da433-124">domainNameService</span></span>|<span data-ttu-id="da433-125">8</span><span class="sxs-lookup"><span data-stu-id="da433-125">8</span></span>|<span data-ttu-id="da433-126">ドメイン ネーム サービス (DNS)。</span><span class="sxs-lookup"><span data-stu-id="da433-126">Domain Name Service (DNS).</span></span>|




