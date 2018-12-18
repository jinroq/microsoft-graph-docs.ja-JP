---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: キラーの資格情報の設定で使用できる値です。
author: tfitzmac
ms.openlocfilehash: 6f6c952d1c480d42db45de6345eba883ff5848a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346964"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="548d0-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="548d0-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="548d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="548d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="548d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="548d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="548d0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="548d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="548d0-107">キラーの資格情報の設定で使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="548d0-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="548d0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="548d0-108">Members</span></span>
|<span data-ttu-id="548d0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="548d0-109">Member</span></span>|<span data-ttu-id="548d0-110">値</span><span class="sxs-lookup"><span data-stu-id="548d0-110">Value</span></span>|<span data-ttu-id="548d0-111">説明</span><span class="sxs-lookup"><span data-stu-id="548d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="548d0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="548d0-112">notConfigured</span></span>|<span data-ttu-id="548d0-113">0</span><span class="sxs-lookup"><span data-stu-id="548d0-113">0</span></span>|<span data-ttu-id="548d0-114">UEFI ロックせずに以前設定されている場合リモート資格情報の保護をオフにします。</span><span class="sxs-lookup"><span data-stu-id="548d0-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="548d0-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="548d0-115">enableWithUEFILock</span></span>|<span data-ttu-id="548d0-116">1</span><span class="sxs-lookup"><span data-stu-id="548d0-116">1</span></span>|<span data-ttu-id="548d0-117">UEFI ロックで資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="548d0-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="548d0-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="548d0-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="548d0-119">2</span><span class="sxs-lookup"><span data-stu-id="548d0-119">2</span></span>|<span data-ttu-id="548d0-120">UEFI ロックせず資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="548d0-120">Turns on Credential Guard without UEFI lock.</span></span>|





