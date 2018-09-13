# <a name="microsoft-graph-security-data-flow"></a>Microsoft Graph Security データのフロー

Microsoft Graph Security API は、Microsoft Graph Security エコシステムのすべてのプロバイダーに対する要求を統合します。 以下の図に示されている通り、これはアプリケーションで提供されるセキュリティ プロバイダーの同意に基づいて行われます。 承認ワークフローは、Microsoft 以外のプロバイダーにのみ適用されます。

![security_dataflow_1.png](./images/security_dataflow_1.png)

フローの説明は次のとおりです。

1. アプリケーションのユーザーは、プロバイダーのアプリケーションにサイン インしてプロバイダーの同意書を表示します。 この同意書または UI はプロバイダーが所有し、Microsoft Graph Security API に要求を送るために、顧客から明確な同意を得る目的でのみ Microsoft 以外のプロバイダーに適用されます。
2. クライアントの同意は、プロバイダー側に保存されます。
3. プロバイダーの同意サービスは、Microsoft Graph Security API を呼び出し、それぞれの顧客に同意を承認するよう通知します。
4. このアプリケーションは、Microsoft Graph Security API に要求を送ります。
5. Microsoft Graph Security API は、さまざまなプロバイダーにマッピングされているこの顧客の同意情報を確認します。
6. Microsoft Graph Security API は、顧客が明確に同意に承認したすべてのプロバイダーを呼び出します。
7. 同意を得たすべてのプロバイダーが、同意した顧客に応答を返します。
8. アプリケーションには、結果を示す応答が返されます。
9. 顧客がプロバイダーの同意を承認しない場合、同意を得られなかったプロバイダーの結果は応答に含まれません。
