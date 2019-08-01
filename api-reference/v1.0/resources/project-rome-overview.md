---
title: Microsoft Graph API を使用してプロジェクトローマを操作する
description: プロジェクトローマは、クロスデバイスエクスペリエンスプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ローカルクライアントまたはサービスのアプリが、クライアントデバイスでのサインインに使用したのと同じ Microsoft アカウントを使用してサインインしたときに、リモートホスト上のアプリとサービスを操作することを可能にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスをプログラミングできます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 03b0aefabdb793cc723b1968a900a35800e04a01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035050"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="dcc12-105">Microsoft Graph API を使用してプロジェクトローマを操作する</span><span class="sxs-lookup"><span data-stu-id="dcc12-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="dcc12-106">[プロジェクトローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、クロスデバイスエクスペリエンスプラットフォームを構築するための Microsoft イニシアティブです。</span><span class="sxs-lookup"><span data-stu-id="dcc12-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="dcc12-107">プロジェクトローマは、ローカルクライアントまたはサービスのアプリが、クライアントデバイスでのサインインに使用したのと同じ Microsoft アカウントを使用してサインインしたときに、リモートホスト上のアプリとサービスを操作することを可能にします。</span><span class="sxs-lookup"><span data-stu-id="dcc12-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="dcc12-108">これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスをプログラミングできます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="dcc12-109">これらのエクスペリエンスを有効にするために、Microsoft Graph を介して重要なコンポーネントが公開されています。アクティビティ。</span><span class="sxs-lookup"><span data-stu-id="dcc12-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="dcc12-110">活アクティビティ</span><span class="sxs-lookup"><span data-stu-id="dcc12-110">Activities</span></span>

<span data-ttu-id="dcc12-111">Microsoft Graph のアクティビティを使用すると、デバイスやプラットフォームを越えてユーザーがアプリを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="dcc12-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="dcc12-112">アクティビティはユーザー契約の単位であり、3つのコンポーネントで構成されます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="dcc12-113">ディープリンク</span><span class="sxs-lookup"><span data-stu-id="dcc12-113">A deep link</span></span>
- <span data-ttu-id="dcc12-114">視覚的な表現</span><span class="sxs-lookup"><span data-stu-id="dcc12-114">A visual representation</span></span>
- <span data-ttu-id="dcc12-115">[https://schema.org/](https://schema.org/)共有ボキャブラリを使用して、アクティビティを記述するコンテンツメタデータ</span><span class="sxs-lookup"><span data-stu-id="dcc12-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="dcc12-116">アプリケーションによってセッションが作成されると、ユーザーの活動期間を反映するために履歴項目がアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="dcc12-117">ユーザーがアクティビティを再実行するたびに、新しい履歴アイテムが、[見越計上] ユーザー契約のアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="dcc12-118">アプリケーションがユーザーアクティビティオブジェクトを公開すると、そのオブジェクトが Windows の新しい UI サーフェスの一部に表示されます。たとえば、Cortana の通知とタイムラインです。</span><span class="sxs-lookup"><span data-stu-id="dcc12-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="dcc12-119">アクティビティオブジェクトでは、リッチメタデータ (アクティビティを正しいコンテキストで表示できるようにする) とリッチビジュアル ([アダプティブカード](https://adaptivecards.io/)マークアップを使用) の両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="dcc12-120">ユーザーアクティビティを作成および取得するには、次の Microsoft Graph Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="dcc12-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="dcc12-121">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="dcc12-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="dcc12-122">アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="dcc12-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="dcc12-123">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="dcc12-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="dcc12-124">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="dcc12-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="dcc12-125">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="dcc12-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="dcc12-126">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="dcc12-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

