---
title: Azure AD と Microsoft Graph のメソッドの相違点
description: Azure Active Directory (Azure AD) Graph API と Microsoft Graph API (REST) との間のメソッドの相違について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 35f97a6c24e0b72200dcd4a37b6fba42ad7ce03d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630238"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD と Microsoft Graph のメソッドの相違点

この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。

Azure AD Graph のいくつかのメソッドも変更されました。  この一覧に表示されていないメソッドは、Azure AD Graph とまったく同じ名前で、既に Microsoft Graph の v1.0[バージョン](/graph/api/overview?view=graph-rest-1.0)で使用できます。

|Azure AD Graph <br>(v 1.6) メソッド |Microsoft Graph<br>(resource/メソッド)|Comments|
|---|---|---|
| getObjectsByObjectId | ベータ&nbsp;-&nbsp;版ディレクトリ/getbyids <br> v 1.0-ディレクトリ/getByIds | |
| restore | &nbsp;-ベータ&nbsp;復元&nbsp;(アプリケーション、&nbsp;ユーザー、&nbsp;および&nbsp;グループ)<br> -&nbsp;&nbsp;&nbsp;v1.0 の復元 (ユーザーと&nbsp;グループ)&nbsp; | また、削除されたアプリケーション、ユーザー、およびグループを表示して、完全に削除することもできます。 |
| invalidateAllRefreshTokens | ベータ-invalidateSigninSessions <br> v 1.0-_まだ使用できません_ | |
| getAvailableExtensionProperties | ベータ-_計画されていません_ <br> v1.0-_計画されていません_ | 現時点では計画されていません。必要に応じて、再検討されることがあります。 |
| isMemberOf | ベータ-_計画されていません_ <br> v1.0-_計画されていません_ | 代わりに、checkMemberGroups を使用してください。 |
| addKey | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | 計画済みですが、まだ使用できません。 | 
| removeKey | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | 計画済みですが、まだ使用できません。 | 
| addPassword | β-addPassword <br> v 1.0-_まだ使用できません_ | |
| removePassword | ベータ-removePassword <br> v 1.0-_まだ使用できません_ | |

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の間でアプリの[API の違いを調べる](migrate-azure-ad-graph-audit-api-use.md)方法について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
