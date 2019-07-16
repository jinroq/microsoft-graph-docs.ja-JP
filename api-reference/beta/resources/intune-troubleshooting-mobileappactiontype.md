---
title: mobileAppActionType 列挙型
description: Intune アプリケーションのアクションの種類を定義します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f2959137eceb8da591f3376b43ad33c10149aa2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740108"
---
# <a name="mobileappactiontype-enum-type"></a><span data-ttu-id="0832a-103">mobileAppActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0832a-103">mobileAppActionType enum type</span></span>

> <span data-ttu-id="0832a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0832a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0832a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0832a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0832a-106">Intune アプリケーションのアクションの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="0832a-106">Defines the Action Types for an Intune Application.</span></span>

## <a name="members"></a><span data-ttu-id="0832a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0832a-107">Members</span></span>
|<span data-ttu-id="0832a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0832a-108">Member</span></span>|<span data-ttu-id="0832a-109">値</span><span class="sxs-lookup"><span data-stu-id="0832a-109">Value</span></span>|<span data-ttu-id="0832a-110">説明</span><span class="sxs-lookup"><span data-stu-id="0832a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0832a-111">不明</span><span class="sxs-lookup"><span data-stu-id="0832a-111">unknown</span></span>|<span data-ttu-id="0832a-112">.0</span><span class="sxs-lookup"><span data-stu-id="0832a-112">0</span></span>|<span data-ttu-id="0832a-113">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="0832a-113">Unknown result.</span></span>|
|<span data-ttu-id="0832a-114">installCommandSent</span><span class="sxs-lookup"><span data-stu-id="0832a-114">installCommandSent</span></span>|<span data-ttu-id="0832a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0832a-115">1</span></span>|<span data-ttu-id="0832a-116">アプリケーションのインストールコマンドが送信されました。</span><span class="sxs-lookup"><span data-stu-id="0832a-116">Application install command was sent.</span></span>|
|<span data-ttu-id="0832a-117">れる</span><span class="sxs-lookup"><span data-stu-id="0832a-117">installed</span></span>|<span data-ttu-id="0832a-118">1/3</span><span class="sxs-lookup"><span data-stu-id="0832a-118">3</span></span>|<span data-ttu-id="0832a-119">アプリケーションがインストールされている。</span><span class="sxs-lookup"><span data-stu-id="0832a-119">Application installed.</span></span>|
|<span data-ttu-id="0832a-120">アンインストール</span><span class="sxs-lookup"><span data-stu-id="0832a-120">uninstalled</span></span>|<span data-ttu-id="0832a-121">2/4</span><span class="sxs-lookup"><span data-stu-id="0832a-121">4</span></span>|<span data-ttu-id="0832a-122">アプリケーションがアンインストールされた。</span><span class="sxs-lookup"><span data-stu-id="0832a-122">Application uninstalled.</span></span>|
|<span data-ttu-id="0832a-123">userRequestedInstall</span><span class="sxs-lookup"><span data-stu-id="0832a-123">userRequestedInstall</span></span>|<span data-ttu-id="0832a-124">5</span><span class="sxs-lookup"><span data-stu-id="0832a-124">5</span></span>|<span data-ttu-id="0832a-125">ユーザーが要求したインストール</span><span class="sxs-lookup"><span data-stu-id="0832a-125">User requested installation</span></span>|




