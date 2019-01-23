---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424225"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="bbe70-103">keyStorageProviderOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="bbe70-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="bbe70-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bbe70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bbe70-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbe70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbe70-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbe70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbe70-107">キー記憶域プロバイダー (KSP) のインポートのオプションです。</span><span class="sxs-lookup"><span data-stu-id="bbe70-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="bbe70-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bbe70-108">Members</span></span>
|<span data-ttu-id="bbe70-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="bbe70-109">Member</span></span>|<span data-ttu-id="bbe70-110">値</span><span class="sxs-lookup"><span data-stu-id="bbe70-110">Value</span></span>|<span data-ttu-id="bbe70-111">説明</span><span class="sxs-lookup"><span data-stu-id="bbe70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbe70-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="bbe70-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="bbe70-113">0</span><span class="sxs-lookup"><span data-stu-id="bbe70-113">0</span></span>|<span data-ttu-id="bbe70-114">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合は、それ以外の場合、ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="bbe70-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="bbe70-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="bbe70-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="bbe70-116">1</span><span class="sxs-lookup"><span data-stu-id="bbe70-116">1</span></span>|<span data-ttu-id="bbe70-117">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合はそれ以外の場合失敗します。</span><span class="sxs-lookup"><span data-stu-id="bbe70-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="bbe70-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="bbe70-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="bbe70-119">2</span><span class="sxs-lookup"><span data-stu-id="bbe70-119">2</span></span>|<span data-ttu-id="bbe70-120">作業 KSP の passport のサイトにインポート可能な場合、失敗します。</span><span class="sxs-lookup"><span data-stu-id="bbe70-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="bbe70-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="bbe70-121">useSoftwareKsp</span></span>|<span data-ttu-id="bbe70-122">3</span><span class="sxs-lookup"><span data-stu-id="bbe70-122">3</span></span>|<span data-ttu-id="bbe70-123">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="bbe70-123">Import to Software KSP.</span></span>|




