---
title: keystorageprovideroption 列挙型
description: キーストレージプロバイダー (KSP) のインポートオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807113"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="20298-103">keystorageprovideroption 列挙型</span><span class="sxs-lookup"><span data-stu-id="20298-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="20298-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20298-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20298-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20298-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20298-106">キーストレージプロバイダー (KSP) のインポートオプション。</span><span class="sxs-lookup"><span data-stu-id="20298-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="20298-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="20298-107">Members</span></span>
|<span data-ttu-id="20298-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="20298-108">Member</span></span>|<span data-ttu-id="20298-109">値</span><span class="sxs-lookup"><span data-stu-id="20298-109">Value</span></span>|<span data-ttu-id="20298-110">説明</span><span class="sxs-lookup"><span data-stu-id="20298-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20298-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="20298-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="20298-112">.0</span><span class="sxs-lookup"><span data-stu-id="20298-112">0</span></span>|<span data-ttu-id="20298-113">トラステッドプラットフォームモジュール (TPM) ksp がある場合は、それ以外の場合は、ソフトウェア ksp にインポートします。</span><span class="sxs-lookup"><span data-stu-id="20298-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="20298-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="20298-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="20298-115">1-d</span><span class="sxs-lookup"><span data-stu-id="20298-115">1</span></span>|<span data-ttu-id="20298-116">トラステッドプラットフォームモジュール (TPM) KSP (存在する場合) にインポートします (それ以外の場合は失敗します)。</span><span class="sxs-lookup"><span data-stu-id="20298-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="20298-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="20298-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="20298-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="20298-118">2</span></span>|<span data-ttu-id="20298-119">利用可能な場合は Passport にインポートし、それ以外の場合は失敗します。</span><span class="sxs-lookup"><span data-stu-id="20298-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="20298-120">その他の方法</span><span class="sxs-lookup"><span data-stu-id="20298-120">useSoftwareKsp</span></span>|<span data-ttu-id="20298-121">1/3</span><span class="sxs-lookup"><span data-stu-id="20298-121">3</span></span>|<span data-ttu-id="20298-122">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="20298-122">Import to Software KSP.</span></span>|





