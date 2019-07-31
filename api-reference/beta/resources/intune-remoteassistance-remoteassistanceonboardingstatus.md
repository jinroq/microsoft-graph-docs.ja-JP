---
title: remoteAssistanceOnboardingStatus 列挙型
description: 現在の TeamViewer connector の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 40d3c7813088370ddffad2fc787d53c96ad0f70b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967567"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="dcb2e-103">remoteAssistanceOnboardingStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="dcb2e-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="dcb2e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcb2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb2e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcb2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb2e-106">現在の TeamViewer connector の状態</span><span class="sxs-lookup"><span data-stu-id="dcb2e-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="dcb2e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dcb2e-107">Members</span></span>
|<span data-ttu-id="dcb2e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dcb2e-108">Member</span></span>|<span data-ttu-id="dcb2e-109">値</span><span class="sxs-lookup"><span data-stu-id="dcb2e-109">Value</span></span>|<span data-ttu-id="dcb2e-110">説明</span><span class="sxs-lookup"><span data-stu-id="dcb2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb2e-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="dcb2e-111">notOnboarded</span></span>|<span data-ttu-id="dcb2e-112">.0</span><span class="sxs-lookup"><span data-stu-id="dcb2e-112">0</span></span>|<span data-ttu-id="dcb2e-113">アクティブな TeamViewer connector が構成されていない場合、またはアクティブである場合に報告される状態</span><span class="sxs-lookup"><span data-stu-id="dcb2e-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="dcb2e-114">契約</span><span class="sxs-lookup"><span data-stu-id="dcb2e-114">onboarding</span></span>|<span data-ttu-id="dcb2e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="dcb2e-115">1</span></span>|<span data-ttu-id="dcb2e-116">システムが TeamViewer 接続を開始したときに報告された状態ですが、サービスはまだコネクタの確認を完了していません。</span><span class="sxs-lookup"><span data-stu-id="dcb2e-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="dcb2e-117">利用</span><span class="sxs-lookup"><span data-stu-id="dcb2e-117">onboarded</span></span>|<span data-ttu-id="dcb2e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="dcb2e-118">2</span></span>|<span data-ttu-id="dcb2e-119">システムが TeamViewer を使用してアカウント情報を正常に交換し、クライアントとのリモートアシスタンスセッションを開始できるようになったときに報告された状態。</span><span class="sxs-lookup"><span data-stu-id="dcb2e-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





