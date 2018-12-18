---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
ms.openlocfilehash: 19c101cc82673009a39d6545f7340fabf65b287a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326615"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="09a87-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="09a87-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="09a87-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09a87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09a87-105">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="09a87-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="09a87-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="09a87-106">Members</span></span>
|<span data-ttu-id="09a87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="09a87-107">Member</span></span>|<span data-ttu-id="09a87-108">値</span><span class="sxs-lookup"><span data-stu-id="09a87-108">Value</span></span>|<span data-ttu-id="09a87-109">説明</span><span class="sxs-lookup"><span data-stu-id="09a87-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a87-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="09a87-110">notConfigured</span></span>|<span data-ttu-id="09a87-111">0</span><span class="sxs-lookup"><span data-stu-id="09a87-111">0</span></span>|<span data-ttu-id="09a87-112">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="09a87-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="09a87-113">高</span><span class="sxs-lookup"><span data-stu-id="09a87-113">high</span></span>|<span data-ttu-id="09a87-114">1</span><span class="sxs-lookup"><span data-stu-id="09a87-114">1</span></span>|<span data-ttu-id="09a87-115">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="09a87-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="09a87-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="09a87-116">highPlus</span></span>|<span data-ttu-id="09a87-117">2</span><span class="sxs-lookup"><span data-stu-id="09a87-117">2</span></span>|<span data-ttu-id="09a87-118">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="09a87-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="09a87-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="09a87-119">zeroTolerance</span></span>|<span data-ttu-id="09a87-120">3</span><span class="sxs-lookup"><span data-stu-id="09a87-120">3</span></span>|<span data-ttu-id="09a87-121">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="09a87-121">Zero tolerance blocks all unknown executables</span></span>|



