---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 283bb12c775b1215a1bcfecf4f248882a56573aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839502"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="f7960-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7960-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="f7960-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7960-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7960-105">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="f7960-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="f7960-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7960-106">Members</span></span>
|<span data-ttu-id="f7960-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7960-107">Member</span></span>|<span data-ttu-id="f7960-108">値</span><span class="sxs-lookup"><span data-stu-id="f7960-108">Value</span></span>|<span data-ttu-id="f7960-109">説明</span><span class="sxs-lookup"><span data-stu-id="f7960-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7960-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f7960-110">notConfigured</span></span>|<span data-ttu-id="f7960-111">0</span><span class="sxs-lookup"><span data-stu-id="f7960-111">0</span></span>|<span data-ttu-id="f7960-112">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="f7960-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="f7960-113">高</span><span class="sxs-lookup"><span data-stu-id="f7960-113">high</span></span>|<span data-ttu-id="f7960-114">1</span><span class="sxs-lookup"><span data-stu-id="f7960-114">1</span></span>|<span data-ttu-id="f7960-115">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="f7960-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="f7960-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="f7960-116">highPlus</span></span>|<span data-ttu-id="f7960-117">2</span><span class="sxs-lookup"><span data-stu-id="f7960-117">2</span></span>|<span data-ttu-id="f7960-118">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="f7960-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="f7960-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="f7960-119">zeroTolerance</span></span>|<span data-ttu-id="f7960-120">3</span><span class="sxs-lookup"><span data-stu-id="f7960-120">3</span></span>|<span data-ttu-id="f7960-121">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f7960-121">Zero tolerance blocks all unknown executables</span></span>|



