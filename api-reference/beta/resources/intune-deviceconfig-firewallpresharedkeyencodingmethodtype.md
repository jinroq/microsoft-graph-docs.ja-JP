---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ddd167d69674c0e32c184aa0f68bd7698331ee3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004303"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="6a7a0-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6a7a0-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="6a7a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a7a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a7a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a7a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7a0-106">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="6a7a0-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="6a7a0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a7a0-107">Members</span></span>
|<span data-ttu-id="6a7a0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a7a0-108">Member</span></span>|<span data-ttu-id="6a7a0-109">値</span><span class="sxs-lookup"><span data-stu-id="6a7a0-109">Value</span></span>|<span data-ttu-id="6a7a0-110">説明</span><span class="sxs-lookup"><span data-stu-id="6a7a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7a0-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6a7a0-111">deviceDefault</span></span>|<span data-ttu-id="6a7a0-112">.0</span><span class="sxs-lookup"><span data-stu-id="6a7a0-112">0</span></span>|<span data-ttu-id="6a7a0-113">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="6a7a0-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="6a7a0-114">none</span><span class="sxs-lookup"><span data-stu-id="6a7a0-114">none</span></span>|<span data-ttu-id="6a7a0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6a7a0-115">1</span></span>|<span data-ttu-id="6a7a0-116">事前共有キーはエンコードされていません。</span><span class="sxs-lookup"><span data-stu-id="6a7a0-116">Preshared key is not encoded.</span></span> <span data-ttu-id="6a7a0-117">代わりに、ワイド文字形式で保存されます。</span><span class="sxs-lookup"><span data-stu-id="6a7a0-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="6a7a0-118">utF8</span><span class="sxs-lookup"><span data-stu-id="6a7a0-118">utF8</span></span>|<span data-ttu-id="6a7a0-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6a7a0-119">2</span></span>|<span data-ttu-id="6a7a0-120">UTF-8 を使用して事前共有キーをエンコードする</span><span class="sxs-lookup"><span data-stu-id="6a7a0-120">Encode the preshared key using UTF-8</span></span>|





