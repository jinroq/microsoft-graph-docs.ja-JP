---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e27ec7042522d7d4c83463b062cdc0c4c109daeb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951412"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="a7522-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a7522-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="a7522-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7522-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7522-105">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="a7522-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="a7522-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7522-106">Members</span></span>
|<span data-ttu-id="a7522-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a7522-107">Member</span></span>|<span data-ttu-id="a7522-108">値</span><span class="sxs-lookup"><span data-stu-id="a7522-108">Value</span></span>|<span data-ttu-id="a7522-109">説明</span><span class="sxs-lookup"><span data-stu-id="a7522-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7522-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a7522-110">notConfigured</span></span>|<span data-ttu-id="a7522-111">0</span><span class="sxs-lookup"><span data-stu-id="a7522-111">0</span></span>|<span data-ttu-id="a7522-112">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="a7522-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="a7522-113">高</span><span class="sxs-lookup"><span data-stu-id="a7522-113">high</span></span>|<span data-ttu-id="a7522-114">1</span><span class="sxs-lookup"><span data-stu-id="a7522-114">1</span></span>|<span data-ttu-id="a7522-115">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="a7522-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="a7522-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="a7522-116">highPlus</span></span>|<span data-ttu-id="a7522-117">2</span><span class="sxs-lookup"><span data-stu-id="a7522-117">2</span></span>|<span data-ttu-id="a7522-118">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="a7522-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="a7522-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="a7522-119">zeroTolerance</span></span>|<span data-ttu-id="a7522-120">3</span><span class="sxs-lookup"><span data-stu-id="a7522-120">3</span></span>|<span data-ttu-id="a7522-121">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="a7522-121">Zero tolerance blocks all unknown executables</span></span>|



