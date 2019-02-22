---
title: keystorageprovideroption 列挙型
description: キーストレージプロバイダー (KSP) のインポートオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddc1cffe1f4e6056d53a151a3b36b2622c9bf4b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153019"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="7b78d-103">keystorageprovideroption 列挙型</span><span class="sxs-lookup"><span data-stu-id="7b78d-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="7b78d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b78d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b78d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b78d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b78d-106">キーストレージプロバイダー (KSP) のインポートオプション。</span><span class="sxs-lookup"><span data-stu-id="7b78d-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="7b78d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7b78d-107">Members</span></span>
|<span data-ttu-id="7b78d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7b78d-108">Member</span></span>|<span data-ttu-id="7b78d-109">値</span><span class="sxs-lookup"><span data-stu-id="7b78d-109">Value</span></span>|<span data-ttu-id="7b78d-110">説明</span><span class="sxs-lookup"><span data-stu-id="7b78d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b78d-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="7b78d-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="7b78d-112">.0</span><span class="sxs-lookup"><span data-stu-id="7b78d-112">0</span></span>|<span data-ttu-id="7b78d-113">トラステッドプラットフォームモジュール (TPM) ksp がある場合は、それ以外の場合は、ソフトウェア ksp にインポートします。</span><span class="sxs-lookup"><span data-stu-id="7b78d-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="7b78d-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="7b78d-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="7b78d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7b78d-115">1</span></span>|<span data-ttu-id="7b78d-116">トラステッドプラットフォームモジュール (TPM) KSP (存在する場合) にインポートします (それ以外の場合は失敗します)。</span><span class="sxs-lookup"><span data-stu-id="7b78d-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="7b78d-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="7b78d-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="7b78d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7b78d-118">2</span></span>|<span data-ttu-id="7b78d-119">利用可能な場合は Passport にインポートし、それ以外の場合は失敗します。</span><span class="sxs-lookup"><span data-stu-id="7b78d-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="7b78d-120">その他の方法</span><span class="sxs-lookup"><span data-stu-id="7b78d-120">useSoftwareKsp</span></span>|<span data-ttu-id="7b78d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7b78d-121">3</span></span>|<span data-ttu-id="7b78d-122">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="7b78d-122">Import to Software KSP.</span></span>|




