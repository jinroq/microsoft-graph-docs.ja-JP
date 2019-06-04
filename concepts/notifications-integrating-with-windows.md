---
title: Windows UWP アプリをユーザー通知用のクライアント側 SDK と統合する
description: Windows UWP アプリをユーザー通知クライアント SDK と統合します。
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: e389e9c319cb2841aa0ddf1dc697134c8c7f4011
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063379"
---
# <a name="integrate-your-windows-uwp-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="44dcb-103">Windows UWP アプリをユーザー通知用のクライアント側 SDK と統合する</span><span class="sxs-lookup"><span data-stu-id="44dcb-103">Integrate your Windows UWP app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="44dcb-104">Azure Portal で[アプリを登録](notifications-integration-app-registration.md)してから、パートナー デベロッパー センターで[クロスデバイス エクスペリエンス](notifications-integration-cross-device-experiences-onboarding.md)を開始したら、その次の手順として、Windows UWP 対応のクライアント側 SDK をクライアント アプリケーションに統合します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK for Windows UWP apps.</span></span>  

<span data-ttu-id="44dcb-105">クライアント側 SDK を使用することで、アプリは、アプリケーション サーバーから現在サインインしているユーザーを対象に発行された通知の受信を開始するために必要な登録手順を実行できるようになります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="44dcb-106">その後で、この SDK はクライアント側での通知の管理を実行します。これには、新しい着信通知の受信、すべて消去のようなシナリオを実現するための通知状態の管理、および完全な通知履歴の取得が含まれます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="44dcb-107">新しい着信通知のフロー</span><span class="sxs-lookup"><span data-stu-id="44dcb-107">New incoming notification flow</span></span>

<span data-ttu-id="44dcb-108">次の図は、新しい着信通知を受信する際のデータ フローを示しています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Windows アプリの新しい通知のフロー](images/notifications-new-notification-windows.png)

<span data-ttu-id="44dcb-110">このプロセスには、いくつかのコンポーネントが関与します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-110">The process involves a few components:</span></span>

* <span data-ttu-id="44dcb-111">アプリケーション サーバー: アプリケーションのバックエンド</span><span class="sxs-lookup"><span data-stu-id="44dcb-111">App server - The back end of your application</span></span>
* <span data-ttu-id="44dcb-112">アプリケーション クライアント: アプリケーションのフロント エンド (UWP アプリ、Android アプリ、または iOS アプリ)</span><span class="sxs-lookup"><span data-stu-id="44dcb-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="44dcb-113">Microsoft Graph 通知: 複数のデバイスおよびプラットフォームに渡って異なるアプリ クライアントのインスタンス間で、ユーザー通知の発行、保存、および同期を可能にするサービス コンポーネント</span><span class="sxs-lookup"><span data-stu-id="44dcb-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="44dcb-114">WNS: クライアントにシグナルを送信するために Microsoft Graph 通知で使用される Windows プッシュ通知サービス</span><span class="sxs-lookup"><span data-stu-id="44dcb-114">WNS - The Windows push notification service that Microsoft Graph notifications uses to signal the clients</span></span>

<span data-ttu-id="44dcb-115">この図は、次の手順を示しています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-115">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="44dcb-116">アプリケーションのロジック。</span><span class="sxs-lookup"><span data-stu-id="44dcb-116">Application logic.</span></span> <span data-ttu-id="44dcb-117">この手順では、ユーザーに通知を発行するトリガーになるものを取り込みます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-117">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="44dcb-118">これは、アプリケーション固有のロジックであり、Microsoft Graph の別のもの (予定表イベントやタスクの割り当てなど) に関するイベントまたはデータの更新になることも、それとは別にアプリ サービスでユーザーに通知しようとしているものになることもあります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-118">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="44dcb-119">アプリケーション サーバーから対象ユーザーへの通知は、Microsoft Graph 通知 API 経由で発行されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-119">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="44dcb-120">詳細については、[サーバー側との統合](notifications-integrating-app-server.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-120">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="44dcb-121">新しい通知が含まれている Web 要求を受信すると、Microsoft Graph 通知は、このアプリとユーザーのためにクラウドで通知の内容を安全に保持します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-121">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="44dcb-122">このユーザーの通知を受信するためにサブスクライブしているアプリのクライアント インスタンスごとに、Microsoft Graph 通知は、オペレーティング システムが提供するネイティブのプッシュ サービスによって、アプリのクライアントに通知するためのシグナルを送信します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-122">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="44dcb-123">ここでは、このアプリケーションは Windows 上の UWP アプリであり、シグナルの送信には [WNS プッシュ直接通知](https://docs.microsoft.com/ja-JP/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview)が使用されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-123">In this case, the application is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
5. <span data-ttu-id="44dcb-124">着信プッシュ通知によるシグナルを受信したアプリケーションは、ユーザー通知ストアでの変更についてフェッチするように SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-124">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="44dcb-125">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-125">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="44dcb-126">SDK は、データの変更 (この場合は新しい通知の内容) を取得します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-126">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="44dcb-127">変更が正常に取得された後、アプリに通知するためのイベント コールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-127">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="44dcb-128">アプリケーションのロジック。</span><span class="sxs-lookup"><span data-stu-id="44dcb-128">Application logic.</span></span> <span data-ttu-id="44dcb-129">この手順では、アプリがイベント コールバック内で実行する内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-129">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="44dcb-130">通常、ローカルのアプリ データが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-130">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="44dcb-131">この場合、通常、アプリは通知内容をユーザーに知らせるトースト通知ポップアップを作成します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-131">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="44dcb-132">通知の更新フロー</span><span class="sxs-lookup"><span data-stu-id="44dcb-132">Notification update flow</span></span>

<span data-ttu-id="44dcb-133">Microsoft Graph 通知を使用する主な利点の 1 つは、通知が安全にクラウドで保持され、ステートフル リソース タイプに変更できることです。</span><span class="sxs-lookup"><span data-stu-id="44dcb-133">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="44dcb-134">そのため、アプリケーションはクロスデバイス シナリオにおいて、サインインしている同一のユーザーに対して、異なるデバイス間で通知の正しい状態を管理および同期できます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-134">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="44dcb-135">あるデバイスで通知が消去または既読になったときには、その他のデバイスにリアルタイムで通知されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-135">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="44dcb-136">"一度処理すれば、すべての場所で消去される" ということが、ユーザーの通知体験の一部として実現されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-136">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="44dcb-137">次の図は、あるデバイスで通知状態の変更や通知の削除があり、その状態の変更や削除を別のデバイスで受信/処理する場合のデータ フローを示しています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-137">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Windows アプリの更新通知のフロー](images/notifications-notification-update-windows.png)

<span data-ttu-id="44dcb-139">このフローの 2 番目の部分は、新しい着信通知の処理のフローと似ています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-139">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="44dcb-140">これは仕様によるものです。SDK のプログラミング パターンでは、あらゆる種類のユーザー通知データの変更 (新規に受信した通知、通知状態の変更、通知の削除など) をアプリケーション クライアントが同じような方法で処理できるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-140">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="44dcb-141">この図は、次の手順を示しています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-141">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="44dcb-142">アプリケーションのロジック。</span><span class="sxs-lookup"><span data-stu-id="44dcb-142">Application logic.</span></span> <span data-ttu-id="44dcb-143">何らかのものが、通知の変更または削除をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="44dcb-143">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="44dcb-144">一般に、あらゆるイベントが通知を変更するトリガーになり得ます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-144">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="44dcb-145">通知を更新または削除するクライアント SDK のアプリによる呼び出し。</span><span class="sxs-lookup"><span data-stu-id="44dcb-145">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="44dcb-146">現在、状態の変更に関して 2 つのプロパティ (**userActionState** および **readState**) が公開されていますが、こうした状態とその状態の更新時期はアプリケーションで定義できます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-146">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="44dcb-147">たとえば、ユーザーが通知ポップアップを消去したときには、**userActionState** が消去済み (Dismissed) になるように更新します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-147">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="44dcb-148">ユーザーが通知ポップアップをクリックして、それに対応するアプリのコンテンツを利用するアプリを起動したときに、**userActionState** をアクティブ化済み (Activated) に更新し、**readState** を読み取り (Read) に更新します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-148">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="44dcb-149">通知を更新または削除するために対応する API が呼び出された後、SDK は、クラウド内のユーザー通知ストアに送信して、この変更をサインインしている同一ユーザーの別のアプリクライアント インスタンスに展開します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-149">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="44dcb-150">クライアントから更新/削除要求を受信した Microsoft Graph 通知は、通知ストアを更新して、この変更をサブスクライブしている別のアプリ クライアント インスタンスを特定します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-150">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="44dcb-151">アプリ クライアントのサブスクリプションごとに、Microsoft Graph 通知は、アプリ クライアントに通知するシグナルを送信します。このとき、オペレーティング システムによって提供されるネイティブ プッシュ サービスが使用されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-151">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="44dcb-152">ここでは、このアプリが Windows 上の UWP アプリであるため、シグナルの送信には [WNS プッシュ直接通知](https://docs.microsoft.com/ja-JP/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview)が使用されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-152">In this case, this is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
6. <span data-ttu-id="44dcb-153">着信プッシュ通知によるシグナルを受信したアプリケーションは、ユーザー通知ストアでの変更についてフェッチするように SDK に求めます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-153">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="44dcb-154">SDK は、Microsoft Graph 内で、ユーザー通知ストアとの安全で準拠した接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-154">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="44dcb-155">SDK によってデータが変更されます。ここでは、変更内容は通知状態の更新または通知の削除です。</span><span class="sxs-lookup"><span data-stu-id="44dcb-155">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="44dcb-156">変更が正常に取得された後、アプリに通知するためのイベント コールバックが SDK で発生します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-156">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="44dcb-157">アプリケーションのロジック。</span><span class="sxs-lookup"><span data-stu-id="44dcb-157">Application logic.</span></span> <span data-ttu-id="44dcb-158">この手順では、アプリがイベント コールバック内で実行する内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-158">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="44dcb-159">通常、ローカルのアプリ データが変更され、ローカルの UI 更新が発生します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-159">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="44dcb-160">ここでは、通知の更新があるため、アプリはローカルに UI を更新して状態の変更を反映させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-160">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="44dcb-161">たとえば、通知にアクティブ化済みのマークが付いている場合は、Windows アクション センター内で対応するトースト通知ポップアップを削除することで、"一度処理すれば、すべての場所で消去" を実現できます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-161">For example, if a notification is marked as activated, you can remove the corresponding toast notification popup inside Windows action center to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="44dcb-162">Microsoft Graph 通知の詳細については、 [Microsoft Graph 通知の概要](notifications-concept-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-162">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="44dcb-163">Microsoft Graph 通知と統合するために必要なすべての手順の詳細については、Microsoft Graph 通知の[統合の概要](notifications-integration-e2e-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-163">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="44dcb-164">プロジェクトに SDK を追加する</span><span class="sxs-lookup"><span data-stu-id="44dcb-164">Adding the references needed to your project</span></span>

<span data-ttu-id="44dcb-165">Windows の場合、このクライアント側 SDK は Windows オペレーティング システムに付属していない NuGet パッケージです。</span><span class="sxs-lookup"><span data-stu-id="44dcb-165">On Windows, the client-side SDK is a NuGet package that ships outside of the Windows operating system.</span></span> <span data-ttu-id="44dcb-166">この API は C#、C++、および WinJS で利用できます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-166">This API is available in C#, C++, and WinJS.</span></span> 

<span data-ttu-id="44dcb-167">Windows アプリ用 Microsoft Graph 通知 SDK に対応する NuGet パッケージを [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications) からダウンロードします。または、Visual Studio で次の手順を使用して、アプリ ソリューションからパッケージをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="44dcb-167">Download the NuGet package for the Microsoft Graph notifications SDK for Windows apps on [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications), or use the following steps to download it from your app solution in Visual Studio:</span></span> 

<span data-ttu-id="44dcb-168">Visual Studio で、プロジェクトを右クリックしてコンテキスト メニューを表示し、**[NuGet パッケージの管理]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="44dcb-168">In Visual Studio, right-click the project to bring up the context menu, and then click **Manage NuGet Packages…**.</span></span>

![NuGet パッケージの管理](images/notifications-nuget-1-manage.png)

<span data-ttu-id="44dcb-170">**[ブラウザー]** タブに移動して、Microsoft.ConnectedDevices.UserNotifications を検索します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-170">Go to the **Browse** tab, and search for Microsoft.ConnectedDevices.UserNotifications.</span></span>

![NuGet パッケージの検索](images/notifications-nuget-2-find.png)

<span data-ttu-id="44dcb-172">検索結果に、Microsoft Graph 通知のクライアント側 SDK が表示されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-172">You will see the Microsoft Graph notifications client-side SDK in the search results.</span></span> <span data-ttu-id="44dcb-173">**[インストール]** ボタンをクリックして、インストールします。</span><span class="sxs-lookup"><span data-stu-id="44dcb-173">Click the **Install** button to install it.</span></span> 

![NuGet パッケージのインストール](images/notifications-nuget-3-install.png)

<span data-ttu-id="44dcb-175">インストールの完了後、このパッケージがソリューション エクスプローラーの **[参照設定]** に表示されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-175">After the installation finishes, the package shows up under **References** in the Solution Explorer.</span></span> 

<span data-ttu-id="44dcb-176">UWP アプリからの NuGet パッケージの組み込みと利用に関する詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-176">For more details about including and consuming NuGet packages from your UWP app, see:</span></span>

* [<span data-ttu-id="44dcb-177">nuget.org からのパッケージの使用</span><span class="sxs-lookup"><span data-stu-id="44dcb-177">Use packages from nuget.org</span></span>](https://docs.microsoft.com/ja-JP/azure/devops/artifacts/nuget/upstream-sources?view=vsts&tabs=new-nav)
* [<span data-ttu-id="44dcb-178">クイックスタート: パッケージのインストールと使用 (Visual Studio)</span><span class="sxs-lookup"><span data-stu-id="44dcb-178">Quickstart: Install and use a package in Visual Studio</span></span>](https://docs.microsoft.com/ja-JP/nuget/quickstart/install-and-use-a-package-in-visual-studio)


## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="44dcb-179">Connected Device Platforms の初期化</span><span class="sxs-lookup"><span data-stu-id="44dcb-179">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="44dcb-180">クライアント側 SDK は、Connected Device Platforms と呼ばれるインフラストラクチャの上に構築されています。</span><span class="sxs-lookup"><span data-stu-id="44dcb-180">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="44dcb-181">どの機能を使用するにしても、まず、このプラットフォームをアプリで初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-181">Before you can use any features, the platform must be initialized within your app.</span></span> <span data-ttu-id="44dcb-182">この初期化手順は、通知シナリオの実行前に必要になるため、メイン クラスの **OnLaunched** メソッドまたは **onActivated** メソッドに配置する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-182">The initialization steps should occur in your main class **OnLaunched** or **onActivated** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="44dcb-183">このプラットフォームの構築と初期化のために、**ConnectedDevicesPlatform** クラスをインスタンス化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-183">You must construct and initialize the platform by instantiating the **ConnectedDevicesPlatform** class.</span></span> <span data-ttu-id="44dcb-184">その前に、次に示すようにイベント ハンドラーがフックされていることを確認してください。これは、プラットフォームの起動後に、イベントがトリガーされる可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="44dcb-184">Before doing that, make sure to hook up event handlers, as shown, because after platform is started, the events might begin to fire.</span></span> 


```C#
var platform = new ConnectedDevicesPlatform();
platform.AccountManager.AccessTokenRequested += AccountManager_AccessTokenRequestedAsync;
platform.AccountManager.AccessTokenInvalidated += AccountManager_AccessTokenInvalidated;
platform.NotificationRegistrationManager.NotificationRegistrationStateChanged += NotificationRegistrationManager_NotificationRegistrationStateChanged;
platform.Start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="44dcb-185">アカウント アクセス トークンの処理</span><span class="sxs-lookup"><span data-stu-id="44dcb-185">Handling account access token</span></span>

<span data-ttu-id="44dcb-186">新しい着信通知のコンテンツの取得、通知状態の更新など、SDK で実行されるすべての Web 呼び出しは、ユーザーのデータに対する読み取りと書き込みになるため、常に有効なアクセス トークンが必要になります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-186">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="44dcb-187">この SDK は、次のイベント (アクセス トークンが要求されたとき、または無効化されたときに起動されるイベント) の処理を必要とします。これにより、プラットフォームの初期化後に、ユーザーのアクセス トークンが正常に処理されるようにします。</span><span class="sxs-lookup"><span data-stu-id="44dcb-187">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accountmanageraccesstokenrequestedasync"></a><span data-ttu-id="44dcb-188">AccountManager_AccessTokenRequestedAsync</span><span class="sxs-lookup"><span data-stu-id="44dcb-188">AccountManager_AccessTokenRequestedAsync</span></span>

<span data-ttu-id="44dcb-189">完全な実装については、[Windows アプリのサンプル](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-189">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void AccountManager_AccessTokenRequestedAsync(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args)
{
    private List<Account> accounts = new List<Account>();
    var account = accounts.Find((x) => x.EqualsTo(args.Request.Account));
    if (account != null)
    {
        try
        {
            var accessToken = await account.GetAccessTokenAsync(args.Request.Scopes);
            args.Request.CompleteWithAccessToken(accessToken);
        }
        catch (Exception ex)
        {
            args.Request.CompleteWithErrorMessage(ex.Message);
        }
    }
}
```

#### <a name="accountmanageraccesstokeninvalidated"></a><span data-ttu-id="44dcb-190">AccountManager_AccessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="44dcb-190">AccountManager_AccessTokenInvalidated</span></span>

<span data-ttu-id="44dcb-191">完全な実装については、[Windows アプリのサンプル](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-191">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private void AccountManager_AccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args)
{
    Logger.Instance.LogMessage($"Token Invalidated. AccountId: {args.Account.Id}, AccountType: {args.Account.Id}, scopes: {string.Join(" ", args.Scopes)}");
}
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="44dcb-192">プッシュ登録の有効期限を処理する</span><span class="sxs-lookup"><span data-stu-id="44dcb-192">Handling push registration expiration</span></span> 

<span data-ttu-id="44dcb-193">Microsoft Graph 通知では、Windows のネイティブ プッシュ プラットフォームである WNS を使用して、ユーザー通知データの変更時にクライアント アプリケーションにシグナルを送信します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-193">Microsoft Graph notifications uses WNS, the native push platform on Windows, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="44dcb-194">これは、新しい着信通知がアプリ サーバーから発行されたときや、クロスデバイス シナリオでサインインしている同一ユーザーの別のデバイスで通知状態が更新されたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-194">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="44dcb-195">そのため、直接プッシュ通知を正常に伝達できる有効な WNS チャネルが必要になります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-195">For this reason, a valid WNS channel that allows raw push notifications to come through successfully is required.</span></span> <span data-ttu-id="44dcb-196">次のイベント コールバックでは、WNS プッシュ チャネルの有効期限切れを処理ます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-196">The following event callback handles WNS push channel expirations.</span></span> 

#### <a name="notificationregistrationmanagernotificationregistrationstatechanged"></a><span data-ttu-id="44dcb-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="44dcb-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span></span>

<span data-ttu-id="44dcb-198">完全な実装については、[Windows アプリのサンプル](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44dcb-198">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void NotificationRegistrationManager_NotificationRegistrationStateChanged(ConnectedDevicesNotificationRegistrationManager sender, ConnectedDevicesNotificationRegistrationStateChangedEventArgs args)
{
    if ((args.State == ConnectedDevicesNotificationRegistrationState.Expired) || (args.State == ConnectedDevicesNotificationRegistrationState.Expiring))
    {
        var account = m_accounts.Find((x) => x.EqualsTo(args.Account));
        if (account != null)
        {
            await account.RegisterAccountWithSdkAsync();
        }
    }
}
```

## <a name="signing-in-your-user"></a><span data-ttu-id="44dcb-199">ユーザーをサインインする</span><span class="sxs-lookup"><span data-stu-id="44dcb-199">Signing in your user</span></span>

<span data-ttu-id="44dcb-200">Microsoft Graph通知は、その他の Microsoft Graph の多くのリソース タイプと同様に、ユーザーが中心になります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-200">Microsoft Graph notifications, like many other resource types inside Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="44dcb-201">サインインしているユーザーの通知にアプリでサブスクライブして受信を開始するには、まず、登録プロセスで使用する有効な OAuth トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-201">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="44dcb-202">OAuth トークンの生成方法と管理方法、は適切なものを選択できます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-202">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="44dcb-203">サンプル アプリでは ADAL を使用します。</span><span class="sxs-lookup"><span data-stu-id="44dcb-203">The sample app uses ADAL.</span></span> 

<span data-ttu-id="44dcb-204">Microsoft アカウントを使用している場合は、サインイン要求に次のアクセス許可を含める必要があります: `wl.offline_access"`、`ccs.ReadWrite`、`wns.connect`、`asimovrome.telemetry`、および `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。</span><span class="sxs-lookup"><span data-stu-id="44dcb-204">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="44dcb-205">Azure AD アカウントを使用している場合は、次の対象ユーザーを要求する必要があります: `https://cdpcs.access.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="44dcb-205">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>


## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="44dcb-206">プラットフォームにユーザー アカウントを追加する</span><span class="sxs-lookup"><span data-stu-id="44dcb-206">Adding the user account to the platform</span></span> 

<span data-ttu-id="44dcb-207">サインインしているユーザーのアカウントを SDK に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-207">You need to register the signed in user account with the SDK.</span></span> <span data-ttu-id="44dcb-208">これには、アカウントの追加と、WNS を通じた初期通知を受信するプッシュ チャネルの登録が伴われます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-208">This involves adding the account and registering a push channel to receive the initial push notifications through WNS.</span></span> 

```C#
var account = new ConnectedDevicesAccount(accountId, accountType);           
var addResult = await platform.AccountManager.AddAccountAsync(account);
if (addResult.Status != ConnectedDevicesAccountAddedStatus.Success)
{
    throw new Exception("Add account failed with " + addResult.Status + "!");
}            

var pushChannel = await PushNotificationChannelManager.CreatePushNotificationChannelForApplicationAsync();
ConnectedDevicesNotificationRegistration registration = new ConnectedDevicesNotificationRegistration();
registration.Type = ConnectedDevicesNotificationType.WNS;
registration.Token = pushChannel.Uri;
var registerResult = await platform.NotificationRegistrationManager.RegisterAsync(account, registration);
if (registerResult.Status != ConnectedDevicesNotificationRegistrationStatus.Success)
{
    throw new Exception("Register push channel failed with " + registerResult.Status + "!");
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="44dcb-209">ユーザーの通知を受信するためのサブスクライブ</span><span class="sxs-lookup"><span data-stu-id="44dcb-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="44dcb-210">このサインインしているユーザーのアプリケーション用に、**UserDataFeed** オブジェクトをインスタンス化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-210">You need to instantiate a **UserDataFeed** object for your application for this signed in user.</span></span> <span data-ttu-id="44dcb-211">アプリケーションは、[クロスデバイス エクスペリエンスの開始時](notifications-integration-cross-device-experiences-onboarding.md)に指定したクロスプラットフォーム アプリ ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md) process.</span></span>

```C#
UserDataFeed feed = UserDataFeed.GetForAccount(account, platform, "YOUR_HOST_HERE");

var scopes = new List<UserDataFeedSyncScope> { UserNotificationChannel.SyncScope };
var subscribeResult = await feed.SubscribeToSyncScopesAsync(scopes);
if (!subscribeResult)
{
    throw new Exception("Subsribe failed!");
}
var channel = new UserNotificationChannel(feed);
var reader = channel.CreateReader();
reader.DataChanged += Reader_DataChanged;
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="44dcb-212">ユーザー通知を受信および管理する</span><span class="sxs-lookup"><span data-stu-id="44dcb-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="44dcb-213">このトピックの前半のフロー図では、アプリ サーバーからの新しい着信通知や、別のアプリケーション クライアント インスタンスで開始された通知の更新または削除を処理するためのプログラミング パターンを示しました。</span><span class="sxs-lookup"><span data-stu-id="44dcb-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="44dcb-214">このようなデータの変更を処理する手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="44dcb-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="44dcb-215">着信プッシュ通知シグナルの処理</span><span class="sxs-lookup"><span data-stu-id="44dcb-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="44dcb-216">すべての種類のユーザー通知データの変更について、アプリ クライアントにプッシュ通知として配信されるシグナルが生成されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="44dcb-217">Windows UWP アプリの場合、このシグナルは WNS プッシュ直接通知として配信されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-217">For Windows UWP apps, the signal is delivered as a WNS push raw notification.</span></span> <span data-ttu-id="44dcb-218">直接プッシュ シグナルの受信時に、アプリでは、**TryParse** を呼び出すことで、Microsoft Graph 通知サービスから実際のデータの変更についてフェッチする SDK をトリガーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-218">On receiving the raw push signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```C#
public async Task ReceiveNotificationAsync(string content)
{
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.TryParse(content);
    if (notification != null)
    {
        await platform.ProcessNotificationAsync(notification);
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="44dcb-219">ユーザー通知のデータ変更の処理</span><span class="sxs-lookup"><span data-stu-id="44dcb-219">Handling user notification data changes</span></span>

<span data-ttu-id="44dcb-220">SDK によってデータ変更が正常にフェッチされると、イベント コールバックが呼び出され、アプリ クライアントによる通知の作成、更新、または削除の処理が求められます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-220">After the SDK successfully fetches the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```C#
private async void Reader_DataChanged(UserNotificationReader reader, object args)
{
    var notifications = await reader.ReadBatchAsync(UInt32.MaxValue);

    foreach (var notification in notifications)
    {
        // Handle notification changes based on change type;
    }
}
```


### <a name="update-state-of-a-notification"></a><span data-ttu-id="44dcb-221">通知の更新状態</span><span class="sxs-lookup"><span data-stu-id="44dcb-221">Update state of a notification</span></span>

<span data-ttu-id="44dcb-222">このアプリ クライアントのインスタンスから通知状態の変更が開始された場合 (たとえば、このデバイスのトースト通知ポップアップをユーザーが有効化した場合)、アプリでは、この状態の変更を同じユーザーが使用するすべてのデバイスで同期するために、SDK を呼び出して通知の状態を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```C#
notification.UserActionState = UserNotificationUserActionState.Activated;
await notification.SaveAsync();
```

### <a name="delete-a-notification"></a><span data-ttu-id="44dcb-223">通知を削除する</span><span class="sxs-lookup"><span data-stu-id="44dcb-223">Delete a notification</span></span>

<span data-ttu-id="44dcb-224">このアプリ クライアントのインスタンスから通知の削除が開始された場合 (たとえば、この通知に対応するタスクに完了のマークが付けられ、アプリのデータベースから通知が削除された場合)、アプリでは、この削除の操作を同じユーザーが使用するすべてのデバイスで同期するために、SDK を呼び出して通知を削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44dcb-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="44dcb-225">通知は、有効期限が切れているか、明示的に削除された場合にのみ、ユーザー通知ストアから削除されます。</span><span class="sxs-lookup"><span data-stu-id="44dcb-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="44dcb-226">**UserActionState** のセマンティック定義はアプリケーション自体によって定義されているため、**UserActionState** が消去済み (Dismissed) になるように更新しても、ユーザー通知は削除されません。</span><span class="sxs-lookup"><span data-stu-id="44dcb-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```C#
await channel.DeleteUserNotificationAsync(notification.Id);
```

## <a name="see-also"></a><span data-ttu-id="44dcb-227">関連項目</span><span class="sxs-lookup"><span data-stu-id="44dcb-227">See also</span></span>

- <span data-ttu-id="44dcb-228">SDK の通知機能に関連する API のフルセットについての [API リファレンス](https://docs.microsoft.com/ja-JP/windows/project-rome/notifications/api-reference-for-windows/)。</span><span class="sxs-lookup"><span data-stu-id="44dcb-228">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-windows/) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="44dcb-229">Windows UWP アプリについての[クライアント側サンプル](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample)。</span><span class="sxs-lookup"><span data-stu-id="44dcb-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample) for Windows UWP apps.</span></span>
- <span data-ttu-id="44dcb-230">通知の発行についての[アプリサーバーのサンプル](notifications-integrating-app-server.md)。</span><span class="sxs-lookup"><span data-stu-id="44dcb-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
