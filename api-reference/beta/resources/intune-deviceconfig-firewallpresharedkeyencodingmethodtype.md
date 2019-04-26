---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: firewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c49a0c97ac8f2e9267f20762fd6e748d952240
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556187"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="c79f2-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c79f2-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="c79f2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c79f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c79f2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c79f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c79f2-106">firewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="c79f2-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c79f2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c79f2-107">Members</span></span>
|<span data-ttu-id="c79f2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c79f2-108">Member</span></span>|<span data-ttu-id="c79f2-109">値</span><span class="sxs-lookup"><span data-stu-id="c79f2-109">Value</span></span>|<span data-ttu-id="c79f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="c79f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c79f2-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="c79f2-111">deviceDefault</span></span>|<span data-ttu-id="c79f2-112">.0</span><span class="sxs-lookup"><span data-stu-id="c79f2-112">0</span></span>|<span data-ttu-id="c79f2-113">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="c79f2-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c79f2-114">なし</span><span class="sxs-lookup"><span data-stu-id="c79f2-114">none</span></span>|<span data-ttu-id="c79f2-115">1 </span><span class="sxs-lookup"><span data-stu-id="c79f2-115">1</span></span>|<span data-ttu-id="c79f2-116">事前共有キーはエンコードされていません。</span><span class="sxs-lookup"><span data-stu-id="c79f2-116">Preshared key is not encoded.</span></span> <span data-ttu-id="c79f2-117">代わりに、ワイド文字形式で保存されます。</span><span class="sxs-lookup"><span data-stu-id="c79f2-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="c79f2-118">utF8</span><span class="sxs-lookup"><span data-stu-id="c79f2-118">utF8</span></span>|<span data-ttu-id="c79f2-119">2 </span><span class="sxs-lookup"><span data-stu-id="c79f2-119">2</span></span>|<span data-ttu-id="c79f2-120">utf-8 を使用して事前共有キーをエンコードする</span><span class="sxs-lookup"><span data-stu-id="c79f2-120">Encode the preshared key using UTF-8</span></span>|





