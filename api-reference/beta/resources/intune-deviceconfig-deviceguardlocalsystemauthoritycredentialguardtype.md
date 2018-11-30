---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: キラーの資格情報の設定で使用できる値です。
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066524"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="153e9-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="153e9-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="153e9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="153e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="153e9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="153e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="153e9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="153e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="153e9-107">キラーの資格情報の設定で使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="153e9-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="153e9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="153e9-108">Members</span></span>
|<span data-ttu-id="153e9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="153e9-109">Member</span></span>|<span data-ttu-id="153e9-110">値</span><span class="sxs-lookup"><span data-stu-id="153e9-110">Value</span></span>|<span data-ttu-id="153e9-111">説明</span><span class="sxs-lookup"><span data-stu-id="153e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="153e9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="153e9-112">notConfigured</span></span>|<span data-ttu-id="153e9-113">0</span><span class="sxs-lookup"><span data-stu-id="153e9-113">0</span></span>|<span data-ttu-id="153e9-114">UEFI ロックせずに以前設定されている場合リモート資格情報の保護をオフにします。</span><span class="sxs-lookup"><span data-stu-id="153e9-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="153e9-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="153e9-115">enableWithUEFILock</span></span>|<span data-ttu-id="153e9-116">1</span><span class="sxs-lookup"><span data-stu-id="153e9-116">1</span></span>|<span data-ttu-id="153e9-117">UEFI ロックで資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="153e9-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="153e9-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="153e9-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="153e9-119">2</span><span class="sxs-lookup"><span data-stu-id="153e9-119">2</span></span>|<span data-ttu-id="153e9-120">UEFI ロックせず資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="153e9-120">Turns on Credential Guard without UEFI lock.</span></span>|





