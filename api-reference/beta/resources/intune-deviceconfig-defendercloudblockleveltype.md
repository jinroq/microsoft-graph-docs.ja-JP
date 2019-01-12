---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 13f8828478eb063eaa25d8561d5a254c86f4b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924721"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="2c77a-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2c77a-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="2c77a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2c77a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c77a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c77a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c77a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c77a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c77a-107">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="2c77a-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="2c77a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2c77a-108">Members</span></span>
|<span data-ttu-id="2c77a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2c77a-109">Member</span></span>|<span data-ttu-id="2c77a-110">値</span><span class="sxs-lookup"><span data-stu-id="2c77a-110">Value</span></span>|<span data-ttu-id="2c77a-111">説明</span><span class="sxs-lookup"><span data-stu-id="2c77a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c77a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2c77a-112">notConfigured</span></span>|<span data-ttu-id="2c77a-113">0</span><span class="sxs-lookup"><span data-stu-id="2c77a-113">0</span></span>|<span data-ttu-id="2c77a-114">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="2c77a-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="2c77a-115">高</span><span class="sxs-lookup"><span data-stu-id="2c77a-115">high</span></span>|<span data-ttu-id="2c77a-116">1</span><span class="sxs-lookup"><span data-stu-id="2c77a-116">1</span></span>|<span data-ttu-id="2c77a-117">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="2c77a-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="2c77a-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="2c77a-118">highPlus</span></span>|<span data-ttu-id="2c77a-119">2</span><span class="sxs-lookup"><span data-stu-id="2c77a-119">2</span></span>|<span data-ttu-id="2c77a-120">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="2c77a-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="2c77a-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="2c77a-121">zeroTolerance</span></span>|<span data-ttu-id="2c77a-122">3</span><span class="sxs-lookup"><span data-stu-id="2c77a-122">3</span></span>|<span data-ttu-id="2c77a-123">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2c77a-123">Zero tolerance blocks all unknown executables</span></span>|





