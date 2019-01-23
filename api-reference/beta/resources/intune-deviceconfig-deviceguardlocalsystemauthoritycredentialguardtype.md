---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: キラーの資格情報の設定で使用できる値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398094"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="90484-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="90484-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="90484-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90484-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90484-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90484-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90484-107">キラーの資格情報の設定で使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="90484-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="90484-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="90484-108">Members</span></span>
|<span data-ttu-id="90484-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="90484-109">Member</span></span>|<span data-ttu-id="90484-110">値</span><span class="sxs-lookup"><span data-stu-id="90484-110">Value</span></span>|<span data-ttu-id="90484-111">説明</span><span class="sxs-lookup"><span data-stu-id="90484-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90484-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="90484-112">notConfigured</span></span>|<span data-ttu-id="90484-113">0</span><span class="sxs-lookup"><span data-stu-id="90484-113">0</span></span>|<span data-ttu-id="90484-114">UEFI ロックせずに以前設定されている場合リモート資格情報の保護をオフにします。</span><span class="sxs-lookup"><span data-stu-id="90484-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="90484-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="90484-115">enableWithUEFILock</span></span>|<span data-ttu-id="90484-116">1</span><span class="sxs-lookup"><span data-stu-id="90484-116">1</span></span>|<span data-ttu-id="90484-117">UEFI ロックで資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="90484-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="90484-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="90484-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="90484-119">2</span><span class="sxs-lookup"><span data-stu-id="90484-119">2</span></span>|<span data-ttu-id="90484-120">UEFI ロックせず資格情報の保護をオンにします。</span><span class="sxs-lookup"><span data-stu-id="90484-120">Turns on Credential Guard without UEFI lock.</span></span>|




