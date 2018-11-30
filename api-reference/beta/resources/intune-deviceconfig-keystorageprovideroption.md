---
title: keyStorageProviderOption 列挙型
description: キー記憶域プロバイダー (KSP) のインポートのオプションです。
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067376"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="f5627-103">keyStorageProviderOption 列挙型</span><span class="sxs-lookup"><span data-stu-id="f5627-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="f5627-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5627-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5627-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5627-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5627-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5627-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5627-107">キー記憶域プロバイダー (KSP) のインポートのオプションです。</span><span class="sxs-lookup"><span data-stu-id="f5627-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="f5627-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f5627-108">Members</span></span>
|<span data-ttu-id="f5627-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f5627-109">Member</span></span>|<span data-ttu-id="f5627-110">値</span><span class="sxs-lookup"><span data-stu-id="f5627-110">Value</span></span>|<span data-ttu-id="f5627-111">説明</span><span class="sxs-lookup"><span data-stu-id="f5627-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5627-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f5627-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="f5627-113">0</span><span class="sxs-lookup"><span data-stu-id="f5627-113">0</span></span>|<span data-ttu-id="f5627-114">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合は、それ以外の場合、ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="f5627-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="f5627-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f5627-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="f5627-116">1</span><span class="sxs-lookup"><span data-stu-id="f5627-116">1</span></span>|<span data-ttu-id="f5627-117">インポートするトラステッド プラットフォーム モジュール (TPM) KSP が存在する場合はそれ以外の場合失敗します。</span><span class="sxs-lookup"><span data-stu-id="f5627-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="f5627-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f5627-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="f5627-119">2</span><span class="sxs-lookup"><span data-stu-id="f5627-119">2</span></span>|<span data-ttu-id="f5627-120">作業 KSP の passport のサイトにインポート可能な場合、失敗します。</span><span class="sxs-lookup"><span data-stu-id="f5627-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="f5627-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f5627-121">useSoftwareKsp</span></span>|<span data-ttu-id="f5627-122">3</span><span class="sxs-lookup"><span data-stu-id="f5627-122">3</span></span>|<span data-ttu-id="f5627-123">ソフトウェア KSP にインポートします。</span><span class="sxs-lookup"><span data-stu-id="f5627-123">Import to Software KSP.</span></span>|





