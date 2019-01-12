---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946554"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="a5bf3-103">keyStorageProviderOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="a5bf3-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="a5bf3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5bf3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5bf3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5bf3-107">キー記憶域プロバイダー (KSP) のインポートのオプションです。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="a5bf3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5bf3-108">Members</span></span>
|<span data-ttu-id="a5bf3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5bf3-109">Member</span></span>|<span data-ttu-id="a5bf3-110">値</span><span class="sxs-lookup"><span data-stu-id="a5bf3-110">Value</span></span>|<span data-ttu-id="a5bf3-111">説明</span><span class="sxs-lookup"><span data-stu-id="a5bf3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5bf3-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a5bf3-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="a5bf3-113">0</span><span class="sxs-lookup"><span data-stu-id="a5bf3-113">0</span></span>|<span data-ttu-id="a5bf3-114">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合は、それ以外の場合、ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="a5bf3-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a5bf3-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="a5bf3-116">1</span><span class="sxs-lookup"><span data-stu-id="a5bf3-116">1</span></span>|<span data-ttu-id="a5bf3-117">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合はそれ以外の場合失敗します。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="a5bf3-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="a5bf3-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="a5bf3-119">2</span><span class="sxs-lookup"><span data-stu-id="a5bf3-119">2</span></span>|<span data-ttu-id="a5bf3-120">作業 KSP の passport のサイトにインポート可能な場合、失敗します。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="a5bf3-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="a5bf3-121">useSoftwareKsp</span></span>|<span data-ttu-id="a5bf3-122">3</span><span class="sxs-lookup"><span data-stu-id="a5bf3-122">3</span></span>|<span data-ttu-id="a5bf3-123">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="a5bf3-123">Import to Software KSP.</span></span>|





