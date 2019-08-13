---
title: mobileAppDependencyType 列挙型
description: 2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b6ed07fb97910d321711ff02d77a231fd796c3a3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322633"
---
# <a name="mobileappdependencytype-enum-type"></a><span data-ttu-id="d0a4d-103">mobileAppDependencyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d0a4d-103">mobileAppDependencyType enum type</span></span>

> <span data-ttu-id="d0a4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0a4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0a4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0a4d-106">2つのモバイルアプリ間の関係に関連付けられている依存関係の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d0a4d-106">Indicates the dependency type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="d0a4d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0a4d-107">Members</span></span>
|<span data-ttu-id="d0a4d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0a4d-108">Member</span></span>|<span data-ttu-id="d0a4d-109">値</span><span class="sxs-lookup"><span data-stu-id="d0a4d-109">Value</span></span>|<span data-ttu-id="d0a4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="d0a4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0a4d-111">検出</span><span class="sxs-lookup"><span data-stu-id="d0a4d-111">detect</span></span>|<span data-ttu-id="d0a4d-112">.0</span><span class="sxs-lookup"><span data-stu-id="d0a4d-112">0</span></span>|<span data-ttu-id="d0a4d-113">親アプリをインストールする前に、子アプリを検出する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d0a4d-113">Indicates that the child app should be detected before installing the parent app.</span></span>|
|<span data-ttu-id="d0a4d-114">自動</span><span class="sxs-lookup"><span data-stu-id="d0a4d-114">autoInstall</span></span>|<span data-ttu-id="d0a4d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d0a4d-115">1</span></span>|<span data-ttu-id="d0a4d-116">親アプリをインストールする前に、子アプリをインストールする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d0a4d-116">Indicates that the child app should be installed before installing the parent app.</span></span>|



