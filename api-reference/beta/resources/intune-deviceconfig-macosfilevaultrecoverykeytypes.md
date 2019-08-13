---
title: macOSFileVaultRecoveryKeyTypes 列挙型
description: MacOS FileVault の回復キーの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1a72cc8ddb4e9ce28a65e3af006ebec097eda247
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365056"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="b1c7a-103">macOSFileVaultRecoveryKeyTypes 列挙型</span><span class="sxs-lookup"><span data-stu-id="b1c7a-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="b1c7a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1c7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c7a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1c7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c7a-106">MacOS FileVault の回復キーの種類</span><span class="sxs-lookup"><span data-stu-id="b1c7a-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="b1c7a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1c7a-107">Members</span></span>
|<span data-ttu-id="b1c7a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1c7a-108">Member</span></span>|<span data-ttu-id="b1c7a-109">値</span><span class="sxs-lookup"><span data-stu-id="b1c7a-109">Value</span></span>|<span data-ttu-id="b1c7a-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1c7a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1c7a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b1c7a-111">notConfigured</span></span>|<span data-ttu-id="b1c7a-112">.0</span><span class="sxs-lookup"><span data-stu-id="b1c7a-112">0</span></span>|<span data-ttu-id="b1c7a-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b1c7a-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="b1c7a-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="b1c7a-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="b1c7a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b1c7a-115">1</span></span>|<span data-ttu-id="b1c7a-116">"マスター" 回復キーは、パスワードが失われたデバイスのロックを解除するために使用できる "マスター" 回復キーに似ています。</span><span class="sxs-lookup"><span data-stu-id="b1c7a-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="b1c7a-117">パーソナル Recoverykey</span><span class="sxs-lookup"><span data-stu-id="b1c7a-117">personalRecoveryKey</span></span>|<span data-ttu-id="b1c7a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b1c7a-118">2</span></span>|<span data-ttu-id="b1c7a-119">個人回復キーは、デバイスに対するパスワードが失われた場合でも、ユーザーのデバイスのロックを解除するために使用できる一意のコードです。</span><span class="sxs-lookup"><span data-stu-id="b1c7a-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



