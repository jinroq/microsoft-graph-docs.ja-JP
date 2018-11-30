---
title: Microsoft Graph でのグループの操作
description: グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有しているユーザーその他のプリンシパルの集合です。 Microsoft Graph では、シナリオに従って、さまざまな種類のグループとグループ機能を作成および管理するために使用できる API を提供します。 Microsoft Graph でのすべてのグループ関連の操作には、管理者の同意が必要です。
ms.openlocfilehash: be0517f4ca13157b1e6e13f52e1500dd47e54afb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021875"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Microsoft Graph でのグループの操作

グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有している[ユーザー](user.md)その他のプリンシパルの集合です。 Microsoft Graph では、シナリオに従って、さまざまな種類のグループとグループ機能を作成および管理するために使用できる API を提供します。 Microsoft Graph でのすべてのグループ関連の操作には、管理者の同意が必要です。

> **注**:グループは、職場または学校のアカウントでのみ作成できます。 個人用 Microsoft アカウントはグループをサポートしません。

| 種類              | 使用例 | groupType | メールが有効 | セキュリティが有効 | API 経由で作成できますか? |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [Office 365 グループ](#office-365-groups) | 共有の Microsoft オンライン リソースを持つユーザーのコラボレーションを容易にします。 | `["Unified"]` | `true` | `false` | はい |
| [セキュリティ グループ](#security-groups-and-mail-enabled-security-groups) | ユーザーのアプリ内リソースへのアクセスを制御します。 | `[]` | `false` | `true` | はい |
| [メールが有効なセキュリティ グループ](#security-groups-and-mail-enabled-security-groups) | 共有グループ メールボックスにより、アプリ内リソースへのユーザー アクセスを制御します。 | `[]` | `true` | `true` | なし |
| 配布グループ | グループのメンバーにメールを配布します。 豊富なリソース セットを提供するため Office 365 グループを使用することをお勧めします。 | `[]` | `true` | `false` | なし |

## <a name="office-365-groups"></a>Office 365 グループ
Office 365 グループのパワーは、共同作業の性質にあり、プロジェクトまたはチームで共同作業するユーザーに最適です。 それは、以下を含む、グループのメンバーが共有するリソースとともに作成されます。

- Outlook 会話
- Outlook カレンダー
- SharePoint ファイル
- OneNote ノートブック
- SharePoint チーム サイト
- Planner の計画
- Intune デバイス管理

### <a name="group-in-outlook-example"></a>Outlook 内のグループ例

Outlook 内にあるグループの JSON 表記を次に示します。 

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```
Office 365 グループと管理者の操作性の詳細については、「[Office 365 グループの概要](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)」を参照してください。

## <a name="security-groups-and-mail-enabled-security-groups"></a>セキュリティ グループとメールが有効なセキュリティ グループ

セキュリティ グループは、リソースへのユーザー アクセスを制御するためのものです。 ユーザーがセキュリティ グループのメンバーであるかどうかを確認することで、そのユーザーがアプリ内のいくつかのセキュア リソースにアクセスしようとしているときに、アプリが承認を判断することができます。 セキュリティ グループには、ユーザーおよび他のセキュリティ グループをメンバーとして含めることができます。

メールが有効なセキュリティ グループは、セキュリティ グループと同じ方法で使用されますが、グループの共有メールボックス機能が追加されています。 API では、メールが有効なセキュリティ グループを作成することはできませんが、他のグループ操作は動作します。  メールが有効なセキュリティ グループは読み取り専用です。 詳細については、「[メールが有効なセキュリティ グループの管理](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx)」の Exchange 記事を参照してください。

### <a name="security-group-example"></a>セキュリティ グループの例

セキュリティ グループの JSON 表記を次に示します。 

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```
## <a name="dynamic-membership"></a>動的メンバーシップ 

すべての種類のグループには、ユーザーのプロパティに基づいてグループから自動的にメンバーを追加または削除する動的メンバーシップ ルールを付けることができます。 たとえば、"マーケティング従業員グループ" には、部署プロパティを "マーケティング" に設定したすべてのユーザーが含まれます。これにより、新たなマーケティング従業員は自動的にグループに追加され、部署を脱退する従業員は自動的にグループから削除されます。 このルールは、グループの作成中に `"membershipRule": 'user.department -eq "Marketing"'` として "membershipRule" フィールドに指定できます。 GroupType には `"DynamicMembership"` も含める必要があります。 次の要求では、マーケティング従業員用の新しい Office 365 グループを作成します。 

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

membershipRule の数式化の詳細については、「[Azure Active Directory で動的グループ メンバーシップの属性ベースのルールを作成する](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)」を参照してください。

> **注**: 動的メンバーシップ ルールには、[Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) 以上の階層のライセンスを持つテナントが必要です。

## <a name="other-types-of-groups"></a>その他の種類のグループ

Yammer の Office 365 グループは、Yammer への投稿によりユーザーのコラボレーションを容易にするために使用されます。 この種類のグループは、読み取りの要求で返すことができますが、その投稿に API でアクセスすることはできません。 Yammer 投稿とスレッド フィードがグループで有効になると、既定の Office 365 グループ会話が無効になります。 詳細については、「[Yammer 開発者向け API ドキュメント](https://developer.yammer.com/docs)」をご覧ください。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph を使用して、次の一般的な操作を実行することができます。

| **ユース ケース**  | **REST リソース** | **関連項目** |
|:---------------|:--------|:----------|
| **グループ オブジェクトおよびメソッド** | | |
| 新しいグループの作成、既存グループの取得、グループでのプロパティの更新、グループの削除を行います。 現在、API を使用して、セキュリティ グループと Outlook 内グループのみを作成できます。 | [group](group.md) | [新しいグループを作成する](../api/group-post-groups.md) <br/> [グループを一覧表示する](../api/group-list.md) <br/> [グループを更新する](../api/group-update.md) <br/> [グループを削除する](../api/group-delete.md) |
| **グループ メンバーシップ メソッド** | | |
| グループのメンバーを一覧表示し、メンバーを追加または削除します。 | [user](user.md) <br/> [group](group.md)| [メンバーを一覧表示する](../api/group-list-members.md) <br/> [メンバーを追加する](../api/group-post-members.md) <br/> [メンバーを削除する](../api/group-delete-members.md)|
| ユーザーがグループのメンバーであるかどうかを判別し、ユーザーがメンバーであるすべてのグループを取得します。 | [user](user.md) <br/> [group](group.md)| [メンバー グループをチェックする](../api/group-checkmembergroups.md) <br/> [メンバー グループを取得する](../api/group-getmembergroups.md)|
| グループの所有者を一覧表示し、所有者を追加または削除します。 | [user](user.md) <br/> [group](group.md)| [所有者を一覧表示する](../api/group-list-members.md) <br/> [メンバーを追加する](../api/group-post-members.md) <br/> [メンバーを削除する](../api/group-delete-members.md)|
