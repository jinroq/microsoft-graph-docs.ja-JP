# <a name="add-custom-data-to-resources-using-extensions"></a>拡張機能を使用してカスタム データをリソースに追加する

Microsoft Graph は、[ユーザー](../api-reference/v1.0/resources/user.md)や[メッセージ](../api-reference/v1.0/resources/message.md)などの数多くのリソースを通じて、多用なユーザー中心のデータと分析情報にアクセスするための単一の API エンドポイントを提供しますします。独自のアプリケーション データを Microsoft Graph で拡張することもできます。外部にデータの保存を必要とせず、Microsoft Graph のリソースにカスタム プロパティを追加できます。

たとえば、**ユーザー** リソースを拡張することによって、アプリを軽量に保ちながら、アプリ固有のユーザー プロファイル データを Microsoft Graph に格納できます。 または、アプリの既存のユーザー プロファイル ストアを保持し、**ユーザー** リソースにアプリ固有のストア識別子を追加することもできます。

Microsoft Graph には、2 種類の拡張機能が備わっています。ご自分のアプリケーションの必要に最適な拡張機能の種類を選択してください。

- **オープン拡張機能**:開発者が使用するのに適しています。
- **スキーマ拡張機能**:型指定されたデータを格納すること、スキーマの検出と共有を容易にすること、フィルターを可能にすること、将来、入力データの検証と承認を可能にすることに関心のある開発者にとって、用途のより広いメカニズムとなります。

> **重要:** 拡張機能は、アカウント資格情報、政府による識別番号、カード名義人データ、財務会計データ、医療情報、機密性のある背景情報などの個人を特定できる機密情報を格納するために使用すべきではありません。

## <a name="supported-resources"></a>サポートされているリソース

次の表は、オープン拡張機能とスキーマ拡張機能をサポートするリソースを示し、それらが一般提供 (GA - v1.0 およびベータ版エンドポイントで提供) されるようになったか、それともプレビュー段階 (ベータ版エンドポイントでのみ提供) かを示します。

|リソース |オープン拡張機能 |スキーマ拡張機能 |
|:------- |:------ |:------ |
| [管理単位](../api-reference/beta/resources/administrativeunit.md) | プレビューのみ | プレビューのみ |
| [予定表イベント](../api-reference/v1.0/resources/event.md) | GA | GA |
| [デバイス](../api-reference/v1.0/resources/device.md) | GA | GA |
| [グループ](../api-reference/v1.0/resources/group.md) | GA | GA |
| [グループ予定表イベント](../api-reference/v1.0/resources/event.md) | GA | GA |
| [グループ会話の投稿](../api-reference/v1.0/resources/post.md) | GA | GA |
| [メッセージ](../api-reference/v1.0/resources/message.md) | GA | GA |
| [組織](../api-reference/v1.0/resources/organization.md) | GA | GA |
| [個人用連絡先](../api-reference/v1.0/resources/contact.md)| GA | GA |
| [ユーザー](../api-reference/v1.0/resources/user.md) | GA | GA |

職場または学校のアカウントを使用してサインインしている場合、これらすべてのリソースについて拡張機能を使用することができます。 また、個人用アカウントでサインインしている場合は、**イベント**、**投稿**、**グループ**、**メッセージ**、**連絡先**、**ユーザー**などのリソースで拡張機能を使用することができます。

## <a name="open-extensions"></a>オープン拡張機能

[オープン拡張機能](../api-reference/v1.0/resources/opentypeextension.md) (以前の Office 365 データ拡張機能) は、[オープン タイプ](http://www.odata.org/getting-started/advanced-tutorial/#openType)であり、型指定されていないアプリ データを直接リソース インスタンスに追加するための柔軟な方法を提供します。

オープン拡張機能は、カスタム データとともに、リソース インスタンスの**拡張機能**ナビゲーション プロパティを介してアクセスできます。
オープン拡張機能で_事前に定義される_書き込み可能なプロパティは、**extensionName** プロパティだけです。 オープン拡張機能を作成する場合、**extensionName** プロパティにテナント内で一意の名前を割り当てる必要があります。

これを行う方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。

拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。

リソース インスタンスに[オープン拡張機能を作成](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)し、すべてのカスタム データを同じ操作で保存することができます (サポートされているリソースの一部については、「[既知の制限](known_issues.md#extensions)」を参照してください)。

その後、拡張機能とそのデータの[読み取り](../api-reference/v1.0/api/opentypeextension_get.md)、[更新](../api-reference/v1.0/api/opentypeextension_update.md)、または[削除](../api-reference/v1.0/api/opentypeextension_delete.md)を行うことができます。

オープン拡張機能の例:[オープン拡張機能を使用したユーザーへのカスタム データの追加](extensibility_open_users.md)

## <a name="schema-extensions"></a>スキーマ拡張機能

[スキーマ拡張機能](../api-reference/v1.0/resources/schemaextension.md)を使用すると、リソースの種類の拡張に使用するスキーマを定義できます。最初に、スキーマ拡張機能の定義を作成します。次に、それを使用して厳密に型指定されたカスタム データを含むリソース インスタンスを拡張します。さらに、スキーマ拡張機能の[状態](#schema-extensions-lifecycle)を制御し、他のアプリで検出できるようにすることができます。これらのアプリでは、そのデータの拡張機能を使用して、エクスペリエンスを拡張して構築できます。

スキーマ拡張機能定義を作成する場合、その **id** の一意の名前を指定する必要があります。次の 2 つの名前付けオプションがあります。

- ご使用のテナントで検証済みのバニティ `.com`、`.net`、`.gov`、`.edu`、`.org` ドメインのいずれかが既にある場合、ドメイン名とスキーマ名を一緒に使用して一意の名前を定義できます (形式: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\})。 たとえば、バニティ ドメインが contoso.com の場合、**id** を `contoso_mySchema` と定義できます。 これは優先オプションです。
- 検証済みバニティ ドメインがない場合、**id** をスキーマ名 (ドメイン名のプレフィックスなし) に設定できます (例: `mySchema`)。Microsoft Graph によって、指定した名前に基づいて文字列 ID が割り当てられます (形式: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\})。例: `extkvbmkofy_mySchema`。

この一意の名前は、拡張リソース インスタンスにカスタム データを格納する複合型の名前として使用される **id** に示されます。

オープン拡張機能とは異なり、スキーマ拡張機能の定義 ([リスト](../api-reference/v1.0/api/schemaextension_list.md)、[作成](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)、[取得](../api-reference/v1.0/api/schemaextension_get.md)、[更新](../api-reference/v1.0/api/schemaextension_update.md)、および[削除](../api-reference/v1.0/api/schemaextension_delete.md)) とそのデータ (データの追加、取得、更新、および削除) の管理は異なるセットの API 操作になっています。

スキーマ拡張機能は、対象となるリソースのインスタンスで複合型としてアクセス可能であるため、次の方法を使用してスキーマ拡張機能でカスタム データの CRUD 操作を行うことができます。

- リソース `POST` メソッドを使用して、新しいリソース インスタンスを作成するときにカスタム データを指定できます。 **連絡先**、**イベント**、**メッセージ**、**投稿**のリソースでは、`PATCH` 操作を使用してスキーマの拡張機能を作成する必要があるという[既知の問題](known_issues.md#creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time)があることにご注意ください。
- リソース `GET` メソッドを使用して、カスタム データを読み取ることができます。
- リソース `PATCH` メソッドを使用して、既存のリソース インスタンスでカスタム データを追加または更新できます。
- リソース `PATCH` メソッドを使用して、複合型を null に設定し、リソース インスタンスのカスタム データを削除できます。

スキーマ拡張機能の例:[スキーマ拡張機能を使用したグループへのカスタム データの追加](extensibility_schema_groups.md)

### <a name="schema-extensions-lifecycle"></a>スキーマ拡張機能のライフサイクル

アプリによってスキーマ拡張機能定義が作成されると、そのアプリがスキーマ拡張機能の所有者としてマークされます。

所有者アプリは、**ステータス** プロパティで PATCH 操作を使用して、拡張機能をさまざまな状態のライフサイクル間で移動できます。所有者アプリは現在の状態に応じて、拡張機能を更新または削除することができます。スキーマ拡張機能の更新は常に、付加的で中断を必要としない更新でなければなりません。

|State |ライフ サイクル状態の動作 |
|:-------------|:------------|
| InDevelopment | <ul><li>作成後の初期状態です。所有者アプリは引き続きスキーマ拡張機能を開発しています。 </li><li>この状態で、所有者のアプリが登録されているディレクトリと同じディレクトリにあるアプリは、このスキーマの定義を持つリソース インスタンスを拡張することができます (アプリにそのリソースへのアクセス許可がある限り)。 </li><li>所有者アプリのみで、拡張機能の定義に追加の変更を加えて更新したり、削除したりできます。 </li><li>所有者アプリは拡張機能を**InDevelopment** から **Available** の状態に移行できます。</li></ul> |
| Available | <ul><li>スキーマ拡張機能は、テナント内のすべてのアプリで利用できます。 </li><li>所有者アプリで拡張機能を **Available** に設定した後、どのアプリでも拡張機能で指定されているこれらのリソースの種類のインスタンスにカスタム データを追加できます (アプリにそのリソースへのアクセス許可がある場合)。 アプリは、新しいインスタンスの作成時または既存のインスタンスの更新時にカスタム データを割り当てることができます。 </li><li>所有者アプリのみで、拡張機能の定義に追加の変更を加えて更新することができます。 この状態では、どのアプリでも拡張機能の定義を削除することはできません。 </li><li>所有者アプリは、スキーマ拡張機能を **Available** から **Deprecated** 状態に移行できます。</li></ul> |
| Deprecated | <ul><li>スキーマ拡張機能の定義の読み取りまたは変更はできなくなります。 </li><li>どのアプリも、新しいプロパティを表示、更新、追加したり、拡張機能を削除したりすることはできません。 </li><li>ただし、既存の拡張機能の_プロパティ値_の読み取り、更新、または削除は引き続き行えます。 </li><li>所有者アプリは、スキーマ拡張機能を **Deprecated** から **Available** 状態に戻すことができます。</li></ul> |

### <a name="supported-property-data-types"></a>サポート対象のプロパティ データ型

スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。

| プロパティの種類 | 注釈 |
|:-------------|:------------|
| Binary | 最大 256 バイトです。 |
| Boolean | メッセージ、イベント、投稿ではサポートされていません。 |
| DateTime | ISO 8601 形式で指定する必要があります。UTC で格納されます。 |
| 整数 | 32 ビット値です。メッセージ、イベント、投稿ではサポートされていません。 |
| String | 最大 256 文字です。 |

> **注:** 複数値プロパティはサポートされていません。

### <a name="azure-ad-directory-schema-extensions"></a>Azure AD ディレクトリのスキーマ拡張機能

Azure AD は、いくつかの [directoryObject](../api-reference/v1.0/resources/directoryObject.md) リソースで、[ディレクトリ スキーマ機能拡張](https://msdn.microsoft.com/ja-JP/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)と呼ばれる、同様の拡張機能をサポートしています。[Azure AD Graph API ](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) を作成して、ディレクトリ スキーマ拡張機能の定義を作成および管理する必要がある場合でも、Microsoft Graph API を使用して、これらの機能拡張プロパティの_データ_を追加、取得、更新、削除することができます。

## <a name="permissions"></a>アクセス許可

特定のリソース上の拡張機能データに対して読み書きするには、そのリソースに対して読み書きするときに必要となるのと同じ[アクセス許可](./permissions_reference.md)が必要になります。 たとえば、サインイン済みのユーザーのプロファイルをカスタム アプリ データで更新できるようにするには、アプリに *User.ReadWrite.All* アクセス許可を付与しておく必要があります。

また、スキーマ拡張機能の定義を作成および管理できるようにするには、アプリケーションに *Directory.AccessAsUser.All* アクセス許可を付与しておく必要があります。

## <a name="data-limits"></a>データの上限

### <a name="open-extension-limits"></a>オープン拡張機能の上限

以下に示す上限がディレクトリ リソース (**ユーザー**、**グループ**、**デバイス**など) に適用されます。

- オープン拡張機能のデータの上限は 2 KB (拡張機能の定義自体を含む) です。
- アプリケーションでは、リソース インスタンスごとに最大 2 つのオープン拡張機能を追加できます。

以下に示す上限が Outlook のリソース (**メッセージ**、**イベント**、**連絡先**など) に適用されます。

- オープン拡張機能のデータは、[MAPI 名前付きプロパティ](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx)に格納され、これは、ユーザーのメールボックスの限られたリソースです。 詳細については、「[openTypeExtension リソースの種類](../api-reference/v1.0/resources/opentypeextension.md)」を参照してください。

### <a name="schema-extension-limits"></a>スキーマの拡張機能の上限

アプリケーションで作成できる**スキーマ拡張機能**の定義は最大 5 つです。

## <a name="known-limitations"></a>既知の制限

拡張機能の使用に関する既知の制限については、既知の問題に関する記事の[「拡張機能」セクション](known_issues.md#extensions)を参照してください。

## <a name="extension-examples"></a>拡張機能の例

- [オープン拡張機能を使用したユーザーへのカスタム データの追加](extensibility_open_users.md)

- [スキーマ拡張機能を使用したグループへのカスタム データの追加](extensibility_schema_groups.md)

## <a name="see-also"></a>関連項目

- [Office 365 のドメイン](https://technet.microsoft.com/ja-JP/library/office-365-domains.aspx)

- [Office 365 テナントのドメインの追加および検証](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
