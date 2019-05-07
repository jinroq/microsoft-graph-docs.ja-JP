---
title: Azure AD Graph Api アプリの使用状況を調べる
description: Azure Active Directory (Azure AD) Api を監査して、アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecf6d1897d8473b42ac8b5bcb45c59747eb36f13
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630273"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Azure AD Graph Api アプリの使用状況を調べる

これは、[アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の手順2です。

Microsoft Graph への移行を計画する際には、既存のアプリケーションを確認し、現在使用している Azure AD Graph Api をカタログ化する時間を取ります。

リストを既知の相違点と比較します。  これにより、アプリを移行するために必要な変更を特定することができます。  これには、エディターの検索と置換機能や、より多くの分析を必要とする複雑な更新プログラムを使用して簡単に解決できる簡単な変更が含まれています。

Microsoft Graph では、Azure AD Graph と同じ機能と機能の多くがサポートされています。  主な違いは次のとおりです。

- [要求の相違点](migrate-azure-ad-graph-request-differences.md)
- [機能の相違点](migrate-azure-ad-graph-feature-differences.md)
- [リソースの種類の違い](migrate-azure-ad-graph-resource-differences.md)
- [プロパティの違い](migrate-azure-ad-graph-property-differences.md)
- [メソッドの違い](migrate-azure-ad-graph-method-differences.md)

アプリが使用している機能に必要なアクセス許可を確認することもできます。  場合によっては、より詳細なアクセス許可を使用できることがあります。

詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[アプリ登録、アクセス許可、および同意の違い](migrate-azure-ad-graph-app-registration.md)について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
