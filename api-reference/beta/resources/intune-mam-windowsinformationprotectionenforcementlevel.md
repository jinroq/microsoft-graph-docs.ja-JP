---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37ec9c781ea4a804260f7dff7b6586c042dcad48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417673"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="f2460-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="f2460-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="f2460-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2460-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2460-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2460-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2460-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2460-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2460-107">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="f2460-107">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="f2460-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2460-108">Members</span></span>
|<span data-ttu-id="f2460-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2460-109">Member</span></span>|<span data-ttu-id="f2460-110">値</span><span class="sxs-lookup"><span data-stu-id="f2460-110">Value</span></span>|<span data-ttu-id="f2460-111">説明</span><span class="sxs-lookup"><span data-stu-id="f2460-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2460-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="f2460-112">noProtection</span></span>|<span data-ttu-id="f2460-113">0</span><span class="sxs-lookup"><span data-stu-id="f2460-113">0</span></span>|<span data-ttu-id="f2460-114">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="f2460-114">No protection enforcement</span></span>|
|<span data-ttu-id="f2460-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="f2460-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="f2460-116">1</span><span class="sxs-lookup"><span data-stu-id="f2460-116">1</span></span>|<span data-ttu-id="f2460-117">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="f2460-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="f2460-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="f2460-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="f2460-119">2</span><span class="sxs-lookup"><span data-stu-id="f2460-119">2</span></span>|<span data-ttu-id="f2460-120">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="f2460-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="f2460-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="f2460-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="f2460-122">3</span><span class="sxs-lookup"><span data-stu-id="f2460-122">3</span></span>|<span data-ttu-id="f2460-123">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="f2460-123">Encrypt, Audit and Block</span></span>|




