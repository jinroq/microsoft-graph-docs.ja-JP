# <a name="office-365-active-users-reports"></a>Office 365 アクティブ ユーザー レポート

Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。 これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot_getoffice365activeuserdetail.md) | Stream      | Office 365 アクティブ ユーザーに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot_getoffice365activeusercounts.md) | Stream      | レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。 |
| [サービスのユーザーの数を取得する](../api/reportroot_getoffice365servicesusercounts.md) | Stream      | アクティビティの種類とサービス別のユーザー数を取得します。 |
