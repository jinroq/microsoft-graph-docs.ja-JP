---
title: fileVaultState 列挙型
description: FileVault 状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f122d62f85f90825f5fe3129ec2a314d5886e6f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726117"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="648b9-103">fileVaultState 列挙型</span><span class="sxs-lookup"><span data-stu-id="648b9-103">fileVaultState enum type</span></span>

> <span data-ttu-id="648b9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="648b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="648b9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="648b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="648b9-106">FileVault 状態</span><span class="sxs-lookup"><span data-stu-id="648b9-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="648b9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="648b9-107">Members</span></span>
|<span data-ttu-id="648b9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="648b9-108">Member</span></span>|<span data-ttu-id="648b9-109">値</span><span class="sxs-lookup"><span data-stu-id="648b9-109">Value</span></span>|<span data-ttu-id="648b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="648b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="648b9-111">success</span><span class="sxs-lookup"><span data-stu-id="648b9-111">success</span></span>|<span data-ttu-id="648b9-112">.0</span><span class="sxs-lookup"><span data-stu-id="648b9-112">0</span></span>|<span data-ttu-id="648b9-113">FileVault の状態の成功</span><span class="sxs-lookup"><span data-stu-id="648b9-113">FileVault State Success</span></span>|
|<span data-ttu-id="648b9-114">ドライブ Encryptedbyuser</span><span class="sxs-lookup"><span data-stu-id="648b9-114">driveEncryptedByUser</span></span>|<span data-ttu-id="648b9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="648b9-115">1</span></span>|<span data-ttu-id="648b9-116">FileVault はユーザーによって有効にされており、ポリシーによって管理されていません</span><span class="sxs-lookup"><span data-stu-id="648b9-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="648b9-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="648b9-117">userDeferredEncryption</span></span>|<span data-ttu-id="648b9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="648b9-118">2</span></span>|<span data-ttu-id="648b9-119">FileVault ポリシーは正しくインストールされていますが、ユーザーは暗号化を開始していません</span><span class="sxs-lookup"><span data-stu-id="648b9-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="648b9-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="648b9-120">escrowNotEnabled</span></span>|<span data-ttu-id="648b9-121">2/4</span><span class="sxs-lookup"><span data-stu-id="648b9-121">4</span></span>|<span data-ttu-id="648b9-122">FileVault 回復キーエスクローが有効になっていません</span><span class="sxs-lookup"><span data-stu-id="648b9-122">FileVault recovery key escrow is not enabled</span></span>|







