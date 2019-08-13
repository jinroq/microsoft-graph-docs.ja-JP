---
title: appListType 列挙型
description: コンプライアンスアプリリストの可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b9166ef625387b47f07b56efd197dc22f1f440d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333907"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="5dc5c-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5dc5c-103">appListType enum type</span></span>

> <span data-ttu-id="5dc5c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dc5c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc5c-106">コンプライアンスアプリリストの可能な値。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="5dc5c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5dc5c-107">Members</span></span>
|<span data-ttu-id="5dc5c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5dc5c-108">Member</span></span>|<span data-ttu-id="5dc5c-109">値</span><span class="sxs-lookup"><span data-stu-id="5dc5c-109">Value</span></span>|<span data-ttu-id="5dc5c-110">説明</span><span class="sxs-lookup"><span data-stu-id="5dc5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc5c-111">none</span><span class="sxs-lookup"><span data-stu-id="5dc5c-111">none</span></span>|<span data-ttu-id="5dc5c-112">.0</span><span class="sxs-lookup"><span data-stu-id="5dc5c-112">0</span></span>|<span data-ttu-id="5dc5c-113">既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-113">Default value, no intent.</span></span>|
|<span data-ttu-id="5dc5c-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="5dc5c-114">appsInListCompliant</span></span>|<span data-ttu-id="5dc5c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5dc5c-115">1</span></span>|<span data-ttu-id="5dc5c-116">リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="5dc5c-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="5dc5c-117">appsNotInListCompliant</span></span>|<span data-ttu-id="5dc5c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5dc5c-118">2</span></span>|<span data-ttu-id="5dc5c-119">このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。</span><span class="sxs-lookup"><span data-stu-id="5dc5c-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



