---
title: windows10VpnAuthenticationMethod 列挙型
description: Windows 10 の VPN 接続の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6159a20c6fc3ad47f3ffc6f78cd3b76e1de1371
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914627"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="3a575-103">windows10VpnAuthenticationMethod 列挙型</span><span class="sxs-lookup"><span data-stu-id="3a575-103">windows10VpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="3a575-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3a575-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a575-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a575-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a575-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a575-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a575-107">Windows 10 の VPN 接続の種類。</span><span class="sxs-lookup"><span data-stu-id="3a575-107">Windows 10 VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="3a575-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3a575-108">Members</span></span>
|<span data-ttu-id="3a575-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3a575-109">Member</span></span>|<span data-ttu-id="3a575-110">値</span><span class="sxs-lookup"><span data-stu-id="3a575-110">Value</span></span>|<span data-ttu-id="3a575-111">説明</span><span class="sxs-lookup"><span data-stu-id="3a575-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a575-112">証明書</span><span class="sxs-lookup"><span data-stu-id="3a575-112">certificate</span></span>|<span data-ttu-id="3a575-113">0</span><span class="sxs-lookup"><span data-stu-id="3a575-113">0</span></span>|<span data-ttu-id="3a575-114">証明書による認証です。</span><span class="sxs-lookup"><span data-stu-id="3a575-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="3a575-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="3a575-115">usernameAndPassword</span></span>|<span data-ttu-id="3a575-116">1</span><span class="sxs-lookup"><span data-stu-id="3a575-116">1</span></span>|<span data-ttu-id="3a575-117">認証用のユーザー名とパスワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="3a575-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="3a575-118">customEapXml</span><span class="sxs-lookup"><span data-stu-id="3a575-118">customEapXml</span></span>|<span data-ttu-id="3a575-119">2</span><span class="sxs-lookup"><span data-stu-id="3a575-119">2</span></span>|<span data-ttu-id="3a575-120">認証方法は、EAP のカスタムの XML で指定されます。</span><span class="sxs-lookup"><span data-stu-id="3a575-120">Authentication method is specified in custom EAP XML.</span></span>|





