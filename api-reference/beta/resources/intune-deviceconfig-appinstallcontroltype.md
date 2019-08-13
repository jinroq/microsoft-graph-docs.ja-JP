---
title: appInstallControlType 列挙型
description: アプリインストールコントロールの設定
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24afb57908ae4b83053474a6c0e069f2ca8f98e6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334032"
---
# <a name="appinstallcontroltype-enum-type"></a><span data-ttu-id="0b6b1-103">appInstallControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b6b1-103">appInstallControlType enum type</span></span>

> <span data-ttu-id="0b6b1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b6b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6b1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b6b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6b1-106">アプリインストールコントロールの設定</span><span class="sxs-lookup"><span data-stu-id="0b6b1-106">App Install control Setting</span></span>

## <a name="members"></a><span data-ttu-id="0b6b1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b6b1-107">Members</span></span>
|<span data-ttu-id="0b6b1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b6b1-108">Member</span></span>|<span data-ttu-id="0b6b1-109">値</span><span class="sxs-lookup"><span data-stu-id="0b6b1-109">Value</span></span>|<span data-ttu-id="0b6b1-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b6b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6b1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0b6b1-111">notConfigured</span></span>|<span data-ttu-id="0b6b1-112">.0</span><span class="sxs-lookup"><span data-stu-id="0b6b1-112">0</span></span>|<span data-ttu-id="0b6b1-113">未構成</span><span class="sxs-lookup"><span data-stu-id="0b6b1-113">Not configured</span></span>|
|<span data-ttu-id="0b6b1-114">箇所</span><span class="sxs-lookup"><span data-stu-id="0b6b1-114">anywhere</span></span>|<span data-ttu-id="0b6b1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0b6b1-115">1</span></span>|<span data-ttu-id="0b6b1-116">アプリの推奨事項をオフにする</span><span class="sxs-lookup"><span data-stu-id="0b6b1-116">Turn off app recommendations</span></span>|
|<span data-ttu-id="0b6b1-117">storeOnly</span><span class="sxs-lookup"><span data-stu-id="0b6b1-117">storeOnly</span></span>|<span data-ttu-id="0b6b1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0b6b1-118">2</span></span>|<span data-ttu-id="0b6b1-119">アプリのみをストアに許可する</span><span class="sxs-lookup"><span data-stu-id="0b6b1-119">Allow apps from Store only</span></span>|
|<span data-ttu-id="0b6b1-120">ガイドライン</span><span class="sxs-lookup"><span data-stu-id="0b6b1-120">recommendations</span></span>|<span data-ttu-id="0b6b1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0b6b1-121">3</span></span>|<span data-ttu-id="0b6b1-122">アプリの推奨事項を表示する</span><span class="sxs-lookup"><span data-stu-id="0b6b1-122">Show me app recommendations</span></span>|
|<span data-ttu-id="0b6b1-123">preferStore</span><span class="sxs-lookup"><span data-stu-id="0b6b1-123">preferStore</span></span>|<span data-ttu-id="0b6b1-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0b6b1-124">4</span></span>|<span data-ttu-id="0b6b1-125">ストアの外部からアプリをインストールする前に警告を表示する</span><span class="sxs-lookup"><span data-stu-id="0b6b1-125">Warn me before installing apps from outside the Store</span></span>|



