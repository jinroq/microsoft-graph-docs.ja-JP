---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
ms.openlocfilehash: c58c844097c18ff86beaef4a0e48d9b8a39043f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317445"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="c8549-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c8549-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="c8549-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8549-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8549-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8549-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8549-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8549-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8549-107">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="c8549-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="c8549-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8549-108">Members</span></span>
|<span data-ttu-id="c8549-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c8549-109">Member</span></span>|<span data-ttu-id="c8549-110">値</span><span class="sxs-lookup"><span data-stu-id="c8549-110">Value</span></span>|<span data-ttu-id="c8549-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8549-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8549-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c8549-112">notConfigured</span></span>|<span data-ttu-id="c8549-113">0</span><span class="sxs-lookup"><span data-stu-id="c8549-113">0</span></span>|<span data-ttu-id="c8549-114">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="c8549-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="c8549-115">高</span><span class="sxs-lookup"><span data-stu-id="c8549-115">high</span></span>|<span data-ttu-id="c8549-116">1</span><span class="sxs-lookup"><span data-stu-id="c8549-116">1</span></span>|<span data-ttu-id="c8549-117">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="c8549-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="c8549-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="c8549-118">highPlus</span></span>|<span data-ttu-id="c8549-119">2</span><span class="sxs-lookup"><span data-stu-id="c8549-119">2</span></span>|<span data-ttu-id="c8549-120">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="c8549-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="c8549-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="c8549-121">zeroTolerance</span></span>|<span data-ttu-id="c8549-122">3</span><span class="sxs-lookup"><span data-stu-id="c8549-122">3</span></span>|<span data-ttu-id="c8549-123">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="c8549-123">Zero tolerance blocks all unknown executables</span></span>|





