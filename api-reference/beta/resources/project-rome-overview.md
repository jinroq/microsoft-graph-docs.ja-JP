---
title: 'Microsoft Graph API を使用してプロジェクトローマを操作する '
description: 'プロジェクトローマは、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。 プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。 これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。 '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbec95682b552210781ecd7390726f8d92c4aa03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965622"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="9bff1-105">Microsoft Graph API を使用してプロジェクトローマを操作する</span><span class="sxs-lookup"><span data-stu-id="9bff1-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bff1-106">[プロジェクトローマ](https://developer.microsoft.com/en-us/windows/project-rome)は、アプリ開発者が強力なクロスデバイスエクスペリエンスを構築できるようにするプラットフォームを構築するための Microsoft イニシアティブです。</span><span class="sxs-lookup"><span data-stu-id="9bff1-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="9bff1-107">プロジェクトローマは、ユーザーが同じ Microsoft アカウントまたは職場または学校のアカウントでサインインしたときに、さまざまなサービスとクライアントエンドポイントを接続するさまざまな機能を有効にします。</span><span class="sxs-lookup"><span data-stu-id="9bff1-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="9bff1-108">これにより、デバイスではなくユーザーのタスクを中心としたクロスデバイスとクロスプラットフォームのエクスペリエンスを実装できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="9bff1-109">Microsoft Graph では、主に3つの主要なプロジェクトローマ機能が提供されています。これにより、大量のクロスデバイスエクスペリエンスを有効にすることができます。アクティビティ、デバイス、および通知。</span><span class="sxs-lookup"><span data-stu-id="9bff1-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="9bff1-110">活アクティビティ</span><span class="sxs-lookup"><span data-stu-id="9bff1-110">Activities</span></span>

<span data-ttu-id="9bff1-111">Microsoft Graph のアクティビティを使用すると、デバイスやプラットフォームを越えてユーザーがアプリを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="9bff1-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="9bff1-112">アクティビティはユーザー契約の単位であり、3つのコンポーネントで構成されます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="9bff1-113">ディープリンク</span><span class="sxs-lookup"><span data-stu-id="9bff1-113">A deep link</span></span>
- <span data-ttu-id="9bff1-114">視覚的な表現</span><span class="sxs-lookup"><span data-stu-id="9bff1-114">A visual representation</span></span>
- <span data-ttu-id="9bff1-115">[https://schema.org/](https://schema.org/)共有ボキャブラリを使用して、アクティビティを記述するコンテンツメタデータ</span><span class="sxs-lookup"><span data-stu-id="9bff1-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="9bff1-116">アプリケーションによってセッションが作成されると、ユーザーの活動期間を反映するために履歴項目がアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="9bff1-117">ユーザーがアクティビティを再実行するたびに、新しい履歴アイテムが、[見越計上] ユーザー契約のアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="9bff1-118">アプリケーションがユーザーアクティビティオブジェクトを公開すると、そのオブジェクトが Windows の新しい UI サーフェスの一部に表示されます。たとえば、Cortana の通知とタイムラインです。</span><span class="sxs-lookup"><span data-stu-id="9bff1-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="9bff1-119">アクティビティオブジェクトでは、リッチメタデータ (アクティビティを正しいコンテキストで表示できるようにする) とリッチビジュアル ([アダプティブカード](https://adaptivecards.io/)マークアップを使用) の両方を指定できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="9bff1-120">ユーザーアクティビティを作成および取得するには、次の Microsoft Graph Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="9bff1-121">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="9bff1-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="9bff1-122">アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="9bff1-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="9bff1-123">最近のアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="9bff1-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="9bff1-124">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="9bff1-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="9bff1-125">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="9bff1-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="9bff1-126">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="9bff1-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="9bff1-127">デバイス</span><span class="sxs-lookup"><span data-stu-id="9bff1-127">Devices</span></span>

<span data-ttu-id="9bff1-128">Microsoft Graph では、次のように Project ローマ Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="9bff1-129">ユーザーのデバイスを検出して接続する</span><span class="sxs-lookup"><span data-stu-id="9bff1-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="9bff1-130">これらのデバイスでアプリをリモートで起動する</span><span class="sxs-lookup"><span data-stu-id="9bff1-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="9bff1-131">これらのデバイス上のアプリにメッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="9bff1-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="9bff1-132">これらの Api を使用して、単一のデバイスを超えする豊富なエクスペリエンスを作成するアプリを構築できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="9bff1-133">たとえば、大きい画面で起動するようにアプリを拡張することができます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="9bff1-134">または、別のユーザーのデバイス上にあるアプリに対してコンパニオン環境を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="9bff1-135">次の Microsoft Graph Api を使用して、他の Windows デバイスと通信できます。</span><span class="sxs-lookup"><span data-stu-id="9bff1-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="9bff1-136">ユーザーのデバイスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9bff1-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="9bff1-137">デバイスにコマンドを送信する</span><span class="sxs-lookup"><span data-stu-id="9bff1-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="9bff1-138">コマンドの状態を取得する</span><span class="sxs-lookup"><span data-stu-id="9bff1-138">Get command status</span></span>](../api/get-device-command-status.md)

