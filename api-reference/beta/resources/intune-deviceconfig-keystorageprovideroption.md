---
title: keyStorageProviderOption 列挙型
description: キーストレージプロバイダー (KSP) のインポートオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77695c9deab823db79a3f8a98df16ff140d87248
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946267"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="9d4b1-103">keyStorageProviderOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="9d4b1-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="9d4b1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d4b1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d4b1-106">キーストレージプロバイダー (KSP) のインポートオプション。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="9d4b1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d4b1-107">Members</span></span>
|<span data-ttu-id="9d4b1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d4b1-108">Member</span></span>|<span data-ttu-id="9d4b1-109">値</span><span class="sxs-lookup"><span data-stu-id="9d4b1-109">Value</span></span>|<span data-ttu-id="9d4b1-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d4b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d4b1-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="9d4b1-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="9d4b1-112">.0</span><span class="sxs-lookup"><span data-stu-id="9d4b1-112">0</span></span>|<span data-ttu-id="9d4b1-113">トラステッドプラットフォームモジュール (TPM) KSP がある場合は、それ以外の場合は、ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="9d4b1-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="9d4b1-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="9d4b1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9d4b1-115">1</span></span>|<span data-ttu-id="9d4b1-116">トラステッドプラットフォームモジュール (TPM) KSP (存在する場合) にインポートします (それ以外の場合は失敗します)。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="9d4b1-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="9d4b1-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="9d4b1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9d4b1-118">2</span></span>|<span data-ttu-id="9d4b1-119">利用可能な場合は Passport にインポートし、それ以外の場合は失敗します。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="9d4b1-120">その他の方法</span><span class="sxs-lookup"><span data-stu-id="9d4b1-120">useSoftwareKsp</span></span>|<span data-ttu-id="9d4b1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9d4b1-121">3</span></span>|<span data-ttu-id="9d4b1-122">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="9d4b1-122">Import to Software KSP.</span></span>|




