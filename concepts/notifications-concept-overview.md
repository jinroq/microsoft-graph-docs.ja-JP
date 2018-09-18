# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Microsoft Graph で通知 API を使用して、人間を中心とした通知を有効にするには 

通知は、ユーザーに従事する最も効果的な方法です。 ユーザーの注意を引いたり、アプリにユーザーを戻します。 マルチ デバイスの世界では、ユーザーは、さまざまなプラットフォームやアプリがあるデバイスなどどこからでも、アプリケーションとサービスにアクセスできます。 

主な目的はユーザーがどこにいても通知することなので、「人間中心」の方法で通知シナリオを設計する必要があります。 主要なプラットフォームで提供されている既存通知ソリューションは、対象とするデバイスには最適です。 Microsoft Graph の通知は、このユーザーを対象化することにより向上します。 Microsoft Graph の通知は、ユーザーとエンドポイント間のマッピング、ユーザーの異なるエンドポイント間の通知状態の同期など、最も手間がかかる部分を処理してくれます。 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>なぜ Microsoft Graph の通知との統合なのですか？
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>異なるエンドポイント間で、ユーザーに通知を配信します
Microsoft グラフの一部として、通知 API を使用すると、Microsoft アカウントまたは作業対象または学校の通知を提供する (Azure AD) アカウントができます。 プラットフォームは、Windows の UWP、Android、iOS など、ユーザーのすべてのエンドポイントにこの通知を配布します。 

### <a name="manage-notifications-across-endpoints"></a>エンドポイント間での通知を管理します
Microsoft Graph 通知 API を使用すると、通知の状態を更新し、すべてのエンドポイント間でその状態を同期させることができます。 たとえば、ユーザーは、1 つのデバイス上の通知の動作 (開封済み、または無視された) などには、この通知の状態を更新することができ、同じ状態の変更は、他のすべてのエンドポイントに配布されます。 Microsoft Graph 通知 API は、ユーザーの通知の状態を一元的な方法で追跡し、通知が一度処理されて、すべての場所で無視されたことの確認を簡単にします。

### <a name="retrieve-notification-history"></a>通知履歴を取得します
通知 API を使用して、定義する有効期限 (最大30日間) に基づく通知履歴を取得できます。 開封済みまたは無視としてマークされている通知は履歴から取得可能で、通知履歴やその他のシナリオのアプリ内表示を有効にします。 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Microsoft Graph での通知 API との統合

いくつかの簡単な手順で Microsoft Graph の通知とアプリを統合することが出来ます - Windows デベロッパー センター経由でアプリをオンボードし、[通知を作成する](../api-reference/beta/api/projectrome_notification_post.md) メソッドを使用して通知を発行し、Project Rome SDK を使用してアプリケーションのクライアントで通知を受信および管理します。  

Microsoft Graph を使用してユーザーの通知を発行する方法の詳細については、 [通知の API リファレンス](../api-reference/beta/resources/notifications-api-overview.md)を参照してください。
 
Project Rome SDK との統合で通知を受信および管理する方法の詳細については、 [Project Rome SDK ドキュメント](https://docs.microsoft.com/en-us/windows/project-rome/)を参照してください。 

## <a name="see-also"></a>関連項目

- [Microsoft Graph のクロスデバイス エクスペリエンス](cross-device-concept-overview.md)
- [Project Rome デベロッパー センター](http://aka.ms/projectrome)
