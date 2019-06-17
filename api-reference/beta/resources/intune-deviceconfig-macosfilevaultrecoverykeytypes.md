---
title: macOSFileVaultRecoveryKeyTypes 列挙型
description: MacOS FileVault の回復キーの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 193bfc5769da2919f93df9beef38524a57bfece0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002547"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="3fd3c-103">macOSFileVaultRecoveryKeyTypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="3fd3c-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="3fd3c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fd3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fd3c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fd3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd3c-106">MacOS FileVault の回復キーの種類</span><span class="sxs-lookup"><span data-stu-id="3fd3c-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="3fd3c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fd3c-107">Members</span></span>
|<span data-ttu-id="3fd3c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fd3c-108">Member</span></span>|<span data-ttu-id="3fd3c-109">値</span><span class="sxs-lookup"><span data-stu-id="3fd3c-109">Value</span></span>|<span data-ttu-id="3fd3c-110">説明</span><span class="sxs-lookup"><span data-stu-id="3fd3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd3c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3fd3c-111">notConfigured</span></span>|<span data-ttu-id="3fd3c-112">.0</span><span class="sxs-lookup"><span data-stu-id="3fd3c-112">0</span></span>|<span data-ttu-id="3fd3c-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="3fd3c-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="3fd3c-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="3fd3c-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="3fd3c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3fd3c-115">1</span></span>|<span data-ttu-id="3fd3c-116">"マスター" 回復キーは、パスワードが失われたデバイスのロックを解除するために使用できる "マスター" 回復キーに似ています。</span><span class="sxs-lookup"><span data-stu-id="3fd3c-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="3fd3c-117">パーソナル Recoverykey</span><span class="sxs-lookup"><span data-stu-id="3fd3c-117">personalRecoveryKey</span></span>|<span data-ttu-id="3fd3c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3fd3c-118">2</span></span>|<span data-ttu-id="3fd3c-119">個人回復キーは、デバイスに対するパスワードが失われた場合でも、ユーザーのデバイスのロックを解除するために使用できる一意のコードです。</span><span class="sxs-lookup"><span data-stu-id="3fd3c-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





